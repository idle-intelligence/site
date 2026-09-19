---
layout: default
title: tts-web
repo: idle-intelligence/tts-web
hf: idle-intelligence/pocket-tts-gguf
demo: https://idle-intelligence.github.io/tts-web/web/
original_model: "kyutai/pocket-tts-without-voice-cloning; KittenML/kitten-tts-nano-0.8-fp32"
dataset: ""
perf_highlight: "Pocket TTS: 2.28x realtime in WASM/Chrome (TTFB 0.41s), M-series Mac — README.md"
blurb: >-
  Browser-native text-to-speech, 100% client-side via Rust/WASM. Two
  engines: Pocket TTS (autoregressive, Mimi codec decoder, streaming) and
  KittenTTS (single forward pass, StyleTTS2 distilled, 14M params). Weights
  on HuggingFace as GGUF/safetensors; 0.23-0.24 RTF native.
---

{{ page.blurb }}
