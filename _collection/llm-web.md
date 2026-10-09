---
layout: card
title: llm-web
kind: code
task_group: LLM inference
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
