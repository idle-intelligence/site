---
layout: card
title: silero-vad-v5-safetensors
kind: model
task_group: Audio codec and VAD
repo: idle-intelligence/vad-rs
hf: idle-intelligence/silero-vad-v5-safetensors
demo: ""
demo_pages: ""
original_model: snakers4/silero-vad
original_author: Silero Team
contribution: Safetensors conversion for candle inference by Idle Intelligence.
dataset: ""
perf_highlight: ""
what_is: Silero VAD v5 weights, converted from ONNX to safetensors for candle inference.
runs: native
model_size: 1.2MB
license: MIT
status: maintained
blurb: >-
  Silero Voice Activity Detection v5 weights, converted from ONNX to safetensors
  for use with candle/Rust inference. Consumed by vad-rs: 16kHz mono PCM in, 512
  samples per call, speech probability out.
---

{{ page.blurb }}
