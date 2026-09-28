---
layout: card
title: t0-alpha-q4_0-webgpu
kind: model
task_group: Forecasting
repo: idle-intelligence/t0-web
hf: idle-intelligence/t0-alpha-q4_0-webgpu
demo: "https://trucs.ai/t0/"
demo_pages: "https://idle-intelligence.github.io/t0-web/web/"
original_model: theforecastingcompany/t0-alpha
dataset: ""
perf_highlight: "GIFT-Eval 97 configs, normalized to Seasonal Naive: MASE 0.7334, CRPS 0.4973"
what_is: Q4_0-quantized weights for t0-alpha, packaged for browser WebGPU forecasting.
runs: browser, WASM, WebGPU
model_size: ~102M params, 58.6 MB (Q4_0)
license: Apache-2.0
status: maintained
blurb: >-
  Smallest, fastest quant of t0-alpha: 29.8 ms per forecast on an Apple M2.
  Costs +1.1% MASE and +0.6% CRPS against the F32 control on the full 97-config
  GIFT-Eval protocol, within 1.3% of the published t0-alpha card. The quant
  trucs.ai/t0/ loads.
---

{{ page.blurb }}
