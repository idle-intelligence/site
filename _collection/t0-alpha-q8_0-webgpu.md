---
layout: card
title: t0-alpha-q8_0-webgpu
kind: model
task_group: Forecasting
repo: idle-intelligence/t0-web
hf: idle-intelligence/t0-alpha-q8_0-webgpu
demo: ""
demo_pages: "https://idle-intelligence.github.io/t0-web/web/"
original_model: theforecastingcompany/t0-alpha
dataset: ""
perf_highlight: "GIFT-Eval 97 configs, normalized to Seasonal Naive: MASE 0.7258, CRPS 0.4943"
what_is: Q8_0-quantized weights for t0-alpha, packaged for browser WebGPU forecasting.
runs: browser, WASM, WebGPU
model_size: ~102M params, 108.9 MB (Q8_0)
license: Apache-2.0
status: maintained
blurb: >-
  Matches the official INT8 export's size (about 109 MB) with less drift from
  the F32 reference (0.20% vs 0.79%) and about 2x its browser forecast speed
  (34.5 ms vs 64.0 ms, Apple M2). Costs +0.04% MASE and +0.02% CRPS against the
  F32 control on GIFT-Eval.
---

{{ page.blurb }}
