---
layout: default
title: llm-life
repo: ""
hf: ""
demo: ""
original_model: Qwen/Qwen2.5-0.5B-Instruct
dataset: ""
perf_highlight: "154.3 ms/cell, batched variant A, WebGPU tab, Apple M2"
what_is: Uses a small language model's logits as the update rule for Conway's Game of Life.
runs: browser, WASM, WebGPU, native
model_size: 0.5B params, Q4_0
license: MIT
status: not yet published
blurb: >-
  Each cell of a Game of Life grid becomes a tiny language-model prompt:
  its neighborhood plus a shared rules prefix. Reading the model's
  confidence per cell, instead of sampling a token, turns its drift from
  the true rule into a picture of the model's own character.
---

{{ page.blurb }}
