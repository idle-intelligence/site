---
layout: card
title: t0-web
kind: code
task_group: Forecasting
repo: idle-intelligence/t0-web
hf: idle-intelligence/t0-alpha-q4_0-webgpu
demo: "https://trucs.ai/t0/"
demo_pages: "https://idle-intelligence.github.io/t0-web/web/"
original_model: theforecastingcompany/t0-alpha; theforecastingcompany/t0-beta
dataset: ""
perf_highlight: 34 ms per forecast (Q8_0, single signal, 512 context) in Chrome on an Apple M2; 30 ms with Q4_0
what_is: A from-scratch port of a probabilistic time-series forecasting transformer to the browser.
runs: native, WASM, WebGPU
model_size: t0-alpha 101.6M params; t0-beta 256M params
license: Apache-2.0
status: maintained
blurb: >-
  Own WGSL implementation of The Forecasting Company's t0 time-series
  forecasters, ported to Burn and wgpu for native and browser use. Weights
  quantize to GGUF Q8_0 and Q4_0 (t0-alpha-q4_0-webgpu, t0-alpha-q8_0-webgpu,
  t0-beta-q4_0-webgpu, t0-beta-q8_0-webgpu), match the PyTorch reference to
  within 1.2e-6, and run in Chrome via WebGPU. A compare page runs this engine
  next to the official ONNX INT8 export side by side in one tab.
---

{{ page.blurb }}
