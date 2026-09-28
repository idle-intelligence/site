---
layout: card
title: kitten-tts-nano-safetensors
kind: model
task_group: Text-to-speech
repo: idle-intelligence/tts-web
hf: idle-intelligence/kitten-tts-nano-safetensors
demo: "https://trucs.ai/tts/"
demo_pages: "https://idle-intelligence.github.io/tts-web/web/"
original_model: KittenML/kitten-tts-nano-0.8
dataset: ""
perf_highlight: ""
what_is: Voice weights for a small text-to-speech model, converted to a Rust-friendly format.
runs: browser, WASM, native
model_size: 14M params, 53MB
license: Apache-2.0
status: maintained
blurb: >-
  KittenTTS nano voice weights converted from ONNX to safetensors for candle
  inference in Rust. A distilled, non-autoregressive StyleTTS2 model with eight
  built-in voices, packaged for both a native CLI and the browser text-to-speech
  demo.
---

{{ page.blurb }}
