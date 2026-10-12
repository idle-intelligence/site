---
layout: card
title: llm-web
kind: code
task_group: LLM and tool calling
repo: idle-intelligence/llm-web
hf: ""
demo: ""
demo_pages: "https://idle-intelligence.github.io/llm-web/web/"
original_model: Qwen/Qwen2.5-0.5B-Instruct
dataset: ""
used_on:
  - title: llm
    url: "https://trucs.ai/llm/"
  - title: llm + tts
    url: "https://trucs.ai/llm-tts/"
  - title: stt + llm + tts
    url: "https://trucs.ai/stt-llm-tts/"
perf_highlight: ""
card_proof: ""
what_is: lean, a small LLM inference engine in Rust and WGSL that runs the same code natively and in the browser.
runs: browser, WASM, WebGPU, native
model_size: 0.5B params, ~430MB (Q4_0 GGUF)
license: "model licence Apache-2.0; code licence MIT"
status: maintained
blurb: >-
  lean is an LLM inference engine written in Rust with WGSL compute kernels on
  wgpu, one codebase that runs natively and compiled to WebAssembly. In the
  browser it picks WebGPU, CPU threads or a single CPU thread depending on what
  the device supports. It loads GGUF weights (Q4_0, Q4_1, Q8_0, Q6_K) for Qwen2,
  Qwen3 and Llama-architecture models, applies LoRA adapters at runtime, and its
  output matches Hugging Face transformers token for token. It is the engine
  behind the trucs.ai chat and voice demos and llm-life's language-model
  methods. The public demo runs SmolLM2-360M-Instruct.
---

{{ page.blurb }}

## How it is built

lean is three Rust crates, each doing one job, compiled from one source to a native library and to WebAssembly, with no ML framework.

```
agent-web, chat pages
  lean-chat   messages to prompt
  lean        text in, text out
  lean-core   the forward pass
```

- **lean-core** is the forward pass. It loads a quantized GGUF model and runs it on the GPU, with hand-written WGSL kernels that keep the weights quantized and dequantize them inside the kernels, or on the CPU, with SIMD dot kernels. It works on token ids and logits, and also holds the KV cache with snapshots and LoRA adapters.
- **lean** is text in, text out. It adds the tokenizer, sampling, the choice of backend, and the reuse of the KV cache for the prefix a new prompt shares with the previous one. It applies no chat template and keeps no conversation.
- **lean-chat** turns chat messages into the prompt text a model expects, with the model's own chat template. The text is byte for byte what transformers' `apply_chat_template` returns, tools included.

Agents such as agent-web sit on top of lean and add the tool-calling loop.

In a browser, lean runs on WebGPU, then on CPU threads, then on a single CPU thread. The choice is made by capability, never by measuring the device. The kernels are the same on every device, with no autotuning and no per-device code. Its output is token-exact against Hugging Face transformers: the greedy tokens match the reference on every backend.
