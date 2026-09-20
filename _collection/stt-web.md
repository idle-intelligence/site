---
layout: default
title: stt-web
repo: idle-intelligence/stt-web
hf: idle-intelligence/stt-1b-en_fr-q4_0-webgpu
demo: https://idle-intelligence.github.io/stt-web/web/
original_model: kyutai/stt-1b-en_fr
dataset: ""
perf_highlight: "~70ms/frame steady state (Mimi ~21ms + STT ~50ms), RTF 0.91-0.95x, Apple M2 (10-core GPU)"
blurb: >-
  Browser-native speech-to-text, 100% client-side via Rust/WASM + WebGPU.
  Microphone audio runs through a Mimi codec (CPU) and a Q4-quantized
  16-layer STT transformer (WebGPU) end to end in Chrome/Edge. Weights are
  quantized from Kyutai's stt-1b-en_fr; not affiliated with Kyutai Labs.
---

{{ page.blurb }}
