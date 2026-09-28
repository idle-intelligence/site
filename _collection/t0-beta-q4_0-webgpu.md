---
layout: card
title: t0-beta-q4_0-webgpu
kind: model
task_group: Forecasting
repo: idle-intelligence/t0-web
hf: idle-intelligence/t0-beta-q4_0-webgpu
demo: ""
demo_pages: "https://idle-intelligence.github.io/t0-web/web/"
original_model: theforecastingcompany/t0-beta
original_author: The Forecasting Company
contribution: Q4_0 quantization for WebGPU by Idle Intelligence.
dataset: ""
perf_highlight: ""
what_is: Q4_0-quantized weights for t0-beta, packaged for browser WebGPU forecasting.
runs: browser, WASM, WebGPU
model_size: 256M params, 149.5 MB (Q4_0)
license: Apache-2.0
status: maintained
blurb: >-
  Smallest, fastest quant of t0-beta: 149.5MB, 0.14x the F32 weights. Worst-case
  point drift against the F32 reference is 14.6%, looser than t0-alpha's own
  Q4_0 (8.4%); no full 97-config GIFT-Eval run exists yet for t0-beta at any
  quant, only an 8-config subset.
---

{{ page.blurb }}
