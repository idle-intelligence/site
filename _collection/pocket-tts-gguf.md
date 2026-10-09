---
layout: card
title: pocket-tts-gguf
kind: model
task_group: Text-to-speech
repo: idle-intelligence/tts-web
hf: idle-intelligence/pocket-tts-gguf
demo: "https://trucs.ai/tts/"
demo_pages: "https://idle-intelligence.github.io/tts-web/web/"
used_on:
  - title: tts
    url: "https://trucs.ai/tts/"
original_model: kyutai/pocket-tts-without-voice-cloning
original_author: Kyutai
contribution: Q8_0 GGUF quantization for the browser by Idle Intelligence.
dataset: ""
perf_highlight: ""
what_is: The GGUF Q8_0 weights, one per language, that tts-web's Pocket TTS engine loads in the browser.
runs: browser, WASM
model_size: ~97M params, 128-134MB per language (Q8_0, decoder path only)
license: CC-BY-4.0
status: maintained
blurb: >-
  Q8_0 GGUF quantization of Kyutai's Pocket TTS in six languages (English,
  French, German, Spanish, Portuguese, Italian), one file per language under
  languages/<name>/ as in Kyutai's repo. Decoder path only (the Mimi
  encoder is excluded, TTS never needs it): transformer backbone, flow matching
  network, Mimi decoder and decoder transformer, shrunk from 236MB to 128MB
  for English.
  Runs via a tiled WASM SIMD128 quantized matmul kernel for about 2x realtime on
  desktop Chrome.
---

{{ page.blurb }}
