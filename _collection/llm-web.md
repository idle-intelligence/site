---
layout: card
title: llm-web
kind: code
task_group: LLM and tool calling
repo: idle-intelligence/llm-web
hf: ""
demo: ""
demo_pages: "https://idle-intelligence.github.io/llm-web/web/"
original_model: Salesforce/xLAM-2-3b-fc-r
dataset: ""
used_on:
  - title: llm
    url: "https://trucs.ai/llm/"
  - title: llm + tts
    url: "https://trucs.ai/llm-tts/"
  - title: stt + llm + tts
    url: "https://trucs.ai/stt-llm-tts/"
perf_highlight: 184 ms/token decode (Q4_0 cooperative matvec kernel, 1.67x speedup over baseline), Apple M2
what_is: Runs a tool-calling language model entirely in the browser, no server required.
runs: browser, WASM, WebGPU
model_size: 3.09B params
license: CC-BY-NC-4.0
status: maintained
blurb: >-
  Self-hosted wllama running LLM inference entirely in the browser via
  WebAssembly, with custom WGSL kernels for Q4_0 quantized matvec/matmul on
  WebGPU. Benchmarked against Salesforce's xLAM-2-3b-fc-r tool-calling model on
  an Apple M2, cutting decode latency from 307ms to 184ms per token. The public
  demo runs a wllama fallback (SmolLM2-360M-Instruct); the Burn+wgpu engine demo
  against xLAM itself is a local dev page, not yet deployed publicly.
---

{{ page.blurb }}
