---
layout: default
title: sts-web
repo: idle-intelligence/sts-web
hf: idle-intelligence/personaplex-24L-q4_k-webgpu
demo: ""
original_model: nvidia/personaplex-7b-v1
dataset: ""
perf_highlight: ""
what_is: A full-duplex speech-to-speech assistant running entirely client-side, still early and rough.
runs: browser, WASM, WebGPU
model_size: 8.37B params, pruned to 24 layers for this build
license: NVIDIA Open Model License
status: experiment
blurb: >-
  Browser-native speech-to-speech, 100% client-side via Rust/WASM + WebGPU.
  Runs a pruned 24-layer, Q4_K-quantized PersonaPlex-7B (QLoRA-recovered
  from NVIDIA's 32-layer original) through a full-duplex pipeline: mic to
  Mimi encoder to temporal/depth transformers to Mimi decoder. Work in
  progress; audio quality is currently poor.
---

{{ page.blurb }}
