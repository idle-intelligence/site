---
layout: card
title: sts-web
kind: code
task_group: Speech-to-speech
repo: idle-intelligence/sts-web
hf: idle-intelligence/personaplex-24L-q4_k-webgpu
demo: ""
demo_pages: "https://idle-intelligence.github.io/sts-web/web/"
original_model: nvidia/personaplex-7b-v1
dataset: ""
used_on:
  - title: sts
    url: "https://trucs.ai/sts/"
perf_highlight: ""
card_proof: "24 of 32 layers, Q4_K"
what_is: A full-duplex speech-to-speech assistant running entirely client-side, still early and rough.
runs: browser, WASM, WebGPU
model_size: 6.74B params (pruned from 8.37B, 24 temporal layers), 3.5GB (Q4_K)
license: "model licence NVIDIA Open Model License; code licence MIT"
status: experiment
blurb: >-
  Browser-native speech-to-speech, 100% client-side via Rust/WASM + WebGPU. Runs
  a pruned 24-layer, Q4_K-quantized PersonaPlex-7B (QLoRA-recovered from
  NVIDIA's 32-layer original) through a full-duplex pipeline: mic to Mimi
  encoder to temporal/depth transformers to Mimi decoder. Walkie-talkie mode
  works with a handful of voice presets; true full-duplex streaming is not
  supported yet, and audio quality is currently poor.
---

{{ page.blurb }}
