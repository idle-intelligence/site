---
layout: card
title: personaplex-24L-q4_k-webgpu
kind: model
task_group: Speech-to-speech
repo: idle-intelligence/sts-web
hf: idle-intelligence/personaplex-24L-q4_k-webgpu
demo: "https://trucs.ai/sts/"
demo_pages: "https://idle-intelligence.github.io/sts-web/web/"
used_on:
  - title: sts
    url: "https://trucs.ai/sts/"
original_model: nvidia/personaplex-7b-v1
original_author: NVIDIA
contribution: Pruned, QLoRA-recovered, Q4_K quantization for WebGPU by Idle Intelligence.
dataset: ""
perf_highlight: ""
what_is: The pruned, QLoRA-recovered, Q4_K-quantized PersonaPlex-7B that sts-web's live demo actually loads.
runs: WebGPU
model_size: 6.74B params (24 of 32 temporal layers), 3.5GB (Q4_K)
license: NVIDIA Open Model License
status: experiment
blurb: >-
  NVIDIA PersonaPlex-7B-v1 with 8 middle temporal-transformer layers removed,
  quality recovered with a rank-32 LoRA trained on self-distilled teacher audio,
  then quantized to Q4_K for browser WebGPU inference. Quality assessed only by
  listening tests so far. Not affiliated with or endorsed by NVIDIA.
---

{{ page.blurb }}
