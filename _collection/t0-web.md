---
layout: default
title: t0-web
repo: ""
hf: ""
demo: ""
original_model: "theforecastingcompany/t0-alpha; theforecastingcompany/t0-beta"
dataset: ""
perf_highlight: "224 ms warm median forward latency (WebGPU/Metal, fusion enabled), Apple M2"
what_is: A from-scratch port of a probabilistic time-series forecasting transformer to the browser.
runs: native, WASM, WebGPU
model_size: "t0-alpha 101.6M params; t0-beta 256M params"
license: Apache-2.0
status: not yet published
blurb: >-
  Own WGSL implementation of The Forecasting Company's t0 time-series
  forecasters, ported to Burn and wgpu for native and browser use. Weights
  quantize to GGUF Q8_0 and Q4_0, match the PyTorch reference to within
  1.2e-6, and already run in headless WebGPU Chromium. A public demo page
  is in progress.
---

{{ page.blurb }}
