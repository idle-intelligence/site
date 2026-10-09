---
layout: card
title: tts-web
kind: code
task_group: Text-to-speech
repo: idle-intelligence/tts-web
hf: idle-intelligence/pocket-tts-gguf
demo: ""
demo_pages: "https://idle-intelligence.github.io/tts-web/web/"
original_model: kyutai/pocket-tts-without-voice-cloning; KittenML/kitten-tts-nano-0.8
dataset: ""
used_on:
  - title: tts
    url: "https://trucs.ai/tts/"
  - title: llm + tts
    url: "https://trucs.ai/llm-tts/"
  - title: stt + llm + tts
    url: "https://trucs.ai/stt-llm-tts/"
perf_highlight: "Pocket TTS: 2.28x realtime in WASM/Chrome (TTFB 0.41s), M-series Mac"
card_proof: "2.28x realtime, WASM/Chrome"
what_is: Converts text to speech in the browser with two lightweight voice models; Pocket TTS speaks six languages.
runs: browser, WASM, native
model_size: Pocket TTS ~100M params; KittenTTS 14M params
license: "model licence CC-BY-4.0 (Pocket TTS), Apache-2.0 (KittenTTS); code licence MIT"
status: maintained
blurb: >-
  Browser-native text-to-speech, 100% client-side via Rust/WASM. Two engines:
  Pocket TTS (autoregressive, Mimi codec decoder, streaming) and KittenTTS
  (single forward pass, StyleTTS2 distilled, 14M params). Weights on HuggingFace
  as GGUF/safetensors; 0.23-0.24 RTF native. Pocket TTS speaks English,
  French, German, Spanish, Portuguese and Italian, each language a Q8_0 GGUF
  quantization (~130MB) of Kyutai's checkpoint, with voices loaded from Kyutai's
  repo at the revision the weights came from. In F32 it matches the official
  implementation frame for frame.
---

{{ page.blurb }}
