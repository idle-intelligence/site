---
layout: default
title: vad-rs
repo: idle-intelligence/vad-rs
hf: idle-intelligence/silero-vad-v5-safetensors
demo: ""
original_model: snakers4/silero-vad
dataset: ""
perf_highlight: ""
blurb: >-
  Silero VAD v5 inference in Rust via candle (CPU tensor ops). Accepts
  24kHz PCM, resamples to 16kHz, and emits SpeechStart/SpeechEnd events
  with configurable thresholds and redemption-frame hysteresis. Weights
  converted from the original ONNX model to safetensors.
---

{{ page.blurb }}
