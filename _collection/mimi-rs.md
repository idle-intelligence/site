---
layout: default
title: mimi-rs
repo: idle-intelligence/mimi-rs
hf: ""
demo: ""
original_model: kyutai/mimi
dataset: ""
perf_highlight: ""
what_is: A Rust implementation of an audio codec that tokenizes and reconstructs speech.
runs: native, WASM
model_size: 96.2M params
license: CC-BY-4.0
status: maintained
blurb: >-
  Rust implementation of Kyutai's Mimi audio codec, built on candle.
  Provides a streaming SEANet encoder/decoder, KV-cached transformer, RVQ
  quantizer, and post-load F32 to Q8_0 weight quantization. Shared library
  powering audio tokenization in tts-web and stt-web's WASM pipelines.
---

{{ page.blurb }}
