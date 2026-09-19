---
layout: default
title: llm-web
repo: idle-intelligence/llm-web
hf: ""
demo: https://idle-intelligence.github.io/llm-web/web/
original_model: Salesforce/xLAM-2-3b-fc-r
dataset: ""
perf_highlight: "184 ms/token decode (Q4_0 cooperative matvec kernel, 1.67x speedup over baseline), Apple M2 — docs/BENCHMARKS.md"
blurb: >-
  Self-hosted wllama running LLM inference entirely in the browser via
  WebAssembly, with custom WGSL kernels for Q4_0 quantized matvec/matmul on
  WebGPU. Benchmarked against Salesforce's xLAM-2-3b-fc-r tool-calling model
  on an Apple M2, cutting decode latency from 307ms to 184ms per token.
---

{{ page.blurb }}
