---
layout: card
title: t0-beta-q8_0-webgpu
kind: model
task_group: Forecasting
repo: idle-intelligence/t0-web
hf: idle-intelligence/t0-beta-q8_0-webgpu
demo: ""
demo_pages: "https://idle-intelligence.github.io/t0-web/web/"
original_model: theforecastingcompany/t0-beta
dataset: ""
perf_highlight: ""
what_is: Q8_0-quantized weights for t0-beta, packaged for browser WebGPU forecasting.
runs: browser, WASM, WebGPU
model_size: 256M params, 275.3 MB (Q8_0)
license: Apache-2.0
status: maintained
blurb: >-
  Matches or beats the official published t0-beta INT8 card: 0.20% worst-case
  mean drift against F32 versus 0.23% for the official card, and much tighter
  point drift (1.06% vs 9.39%). No browser measurement exists yet; only native
  Metal latency has been measured.
---

{{ page.blurb }}
