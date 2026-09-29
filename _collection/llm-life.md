---
layout: card
title: llm-life
kind: code
task_group: Cellular automata
repo: idle-intelligence/llm-life
hf: idle-intelligence/llm-of-life-lora
demo: ""
demo_pages: "https://idle-intelligence.github.io/llm-life/web/"
original_model: Qwen/Qwen2.5-0.5B-Instruct
dataset: ""
perf_highlight: 31.97 s/generation (LLM per cell, trained, batched), 256/256 cells correct, 16x16 grid, browser tab, Apple M2
what_is: Uses a small language model's logits as the update rule for Conway's Game of Life.
runs: browser, WASM, WebGPU, native
model_size: 0.5B params, Q4_0
license: MIT
status: maintained
blurb: >-
  Each cell of a Game of Life grid becomes a tiny language-model prompt: its
  neighborhood plus a shared rules prefix. Reading the model's confidence per
  cell, instead of sampling a token, turns its drift from the true rule into a
  picture of the model's own character. The same repo trains three from-scratch
  alternatives on the same task: a 3,490-parameter BERT-style classifier, a
  1,442-parameter MLP, and a 3,329-parameter stencil-attention model that solves
  the whole grid in one pass, collected in stencil-life. A compare page runs
  every method on the same grid, one tab.
---

{{ page.blurb }}

Measured in a browser tab at 16x16 on an M2:

| method | s / generation | parameters | cells correct |
|---|---|---|---|
| Game of Life (rule) | 5.43e-6 | no parameters | 256 / 256 |
| lookup table | 2.98e-6 | 512-entry table | 256 / 256 |
| LLM per cell (trained) | 28.46 | 0.5B (+ adapter) | 256 / 256 |
| LLM whole grid (trained) | 0.6364 | 0.5B (+ adapter) | 256 / 256 |
| BERT of Life (batched) | 0.0195 | 3,490 | 256 / 256 |
| 9 numbers to centre (batched) | 0.0253 | 1,442 | 256 / 256 |
| stencil (grid to grid) | 0.0928 | 3,329 | 256 / 256 |
