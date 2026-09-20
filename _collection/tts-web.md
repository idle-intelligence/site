---
layout: default
title: tts-web
repo: idle-intelligence/tts-web
hf: idle-intelligence/pocket-tts-gguf
demo: https://trucs.ai/tts/
original_model: "kyutai/pocket-tts-without-voice-cloning; KittenML/kitten-tts-nano-0.8-fp32"
dataset: ""
perf_highlight: "Pocket TTS: 2.28x realtime in WASM/Chrome (TTFB 0.41s), M-series Mac"
what_is: Converts text to speech in the browser, with two interchangeable lightweight voice models.
runs: browser, WASM, native
model_size: "Pocket TTS ~100M params; KittenTTS 14M params"
license: "CC-BY-4.0 (Pocket TTS); Apache-2.0 (KittenTTS)"
status: maintained
blurb: >-
  Browser-native text-to-speech, 100% client-side via Rust/WASM. Two
  engines: Pocket TTS (autoregressive, Mimi codec decoder, streaming) and
  KittenTTS (single forward pass, StyleTTS2 distilled, 14M params). Weights
  on HuggingFace as GGUF/safetensors; 0.23-0.24 RTF native.
---

{{ page.blurb }}
