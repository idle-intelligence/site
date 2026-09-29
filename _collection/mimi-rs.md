---
layout: card
title: mimi-rs
kind: code
task_group: Audio codec and VAD
repo: idle-intelligence/mimi-rs
hf: ""
demo: ""
demo_pages: ""
original_model: kyutai/mimi
dataset: ""
perf_highlight: ""
card_proof: "96.2M params"
what_is: A Rust implementation of an audio codec that tokenizes and reconstructs speech.
runs: browser, WASM, native
model_size: 96.2M params
license: CC-BY-4.0
status: maintained
blurb: >-
  Rust implementation of Kyutai's Mimi audio codec, built on candle. Provides a
  streaming SEANet encoder/decoder, KV-cached transformer, RVQ quantizer, and
  post-load F32 to Q8_0 weight quantization. Shared library powering audio
  tokenization in tts-web and stt-web's WASM pipelines.
---

{{ page.blurb }}
