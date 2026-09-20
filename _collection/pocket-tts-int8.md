---
layout: default
title: pocket-tts-int8
repo: ""
hf: idle-intelligence/pocket-tts-int8
demo: ""
original_model: kyutai/pocket-tts-without-voice-cloning
dataset: ""
perf_highlight: ""
what_is: An INT8-quantized version of a lightweight autoregressive text-to-speech model.
runs: browser, WASM
model_size: 100M params, 132MB (channel-wise INT8, 41% smaller than the original)
license: CC-BY-4.0
status: maintained
blurb: >-
  Channel-wise INT8 quantization of Kyutai's Pocket TTS, shrinking the
  weights from 225MB to 132MB for faster loading in browser-based
  text-to-speech inference via WebAssembly.
---

{{ page.blurb }}
