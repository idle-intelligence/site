---
layout: card
title: stt-1b-en_fr-q4_0-webgpu
kind: model
task_group: Speech-to-text
repo: idle-intelligence/stt-web
hf: idle-intelligence/stt-1b-en_fr-q4_0-webgpu
demo: "https://trucs.ai/stt/"
demo_pages: "https://idle-intelligence.github.io/stt-web/web/"
original_model: kyutai/stt-1b-en_fr
original_author: Kyutai
contribution: Q4_0 quantization for WebGPU by Idle Intelligence.
dataset: ""
perf_highlight: ""
what_is: Q4-quantized weights for a ~1B-parameter streaming speech-to-text transformer, packaged for the browser.
runs: browser, WASM, WebGPU
model_size: ~1B + ~25M params, 638MB total (Q4_0 + f16)
license: CC-BY-4.0
status: maintained
blurb: >-
  Q4-quantized weights for kyutai/stt-1b-en_fr, packaged for client-side browser
  inference via WASM + WebGPU: English and French, streaming, about 1B
  parameters. Consumed by stt-web; not affiliated with or endorsed by Kyutai
  Labs.
---

{{ page.blurb }}
