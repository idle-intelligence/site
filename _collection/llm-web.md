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
perf_highlight: "76.7% tool-calling accuracy with schema-constrained decoding vs 53.3% unconstrained, 43-utterance eval"
what_is: Runs a tool-calling language model entirely in the browser, no server required.
runs: browser, WASM, WebGPU
model_size: 0.5B params, ~430MB (Q4_0 GGUF)
license: "model licence Apache-2.0; code licence MIT"
status: maintained
blurb: >-
  An original Burn and wgpu implementation of the Qwen2 architecture, compiled
  to WebAssembly and running the full forward pass client-side with WebGPU:
  quantized GGUF weights, runtime LoRA adapters, schema-constrained decoding for
  tool calls, and a multi-step agent loop. Runs Qwen2.5-0.5B-Instruct in the
  browser with runtime LoRA adapters, the same engine behind llm-life's
  language-model methods. The public demo runs a wllama fallback
  (SmolLM2-360M-Instruct); the Burn+wgpu engine demo is a local dev page, not
  yet deployed publicly.
---

{{ page.blurb }}
