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
perf_highlight: 8.48 s/generation (LLM per cell, trained, batched, on lean), 256/256 cells correct, 16x16 grid, browser tab, Apple M2
card_proof: "256/256 cells, 7 methods compared"
what_is: Uses a small language model's logits as the update rule for Conway's Game of Life.
runs: browser, WASM, WebGPU, native
model_size: 0.5B params, Q4_0
license: "model licence Apache-2.0; code licence MIT"
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

Measured in a browser tab at 16x16 on an M2, one generation per row:

| method | s / generation | parameters | cells correct |
|---|---|---|---|
| Game of Life (rule) | 5.40e-6 | no parameters | 256 / 256 |
| lookup table | 3.23e-6 | 512-entry table | 256 / 256 |
| LLM per cell (trained) | 17.09 | 0.5B (+ adapter) | 256 / 256 |
| LLM whole grid (trained) | 0.4971 | 0.5B (+ adapter) | 256 / 256 |
| BERT of Life (batched) | 0.0173 | 3,490 | 256 / 256 |

At 2048x2048 the language models are left out and the grid goes to the graphics processor. Measured in a Chromium browser tab on an Apple M2 with WebGPU, 200 generations per row from the same starting board, each final board checked cell by cell against the rule. Read back means the board returns to the CPU after every generation, kept there means it stays on the GPU, and bitwise packs 32 cells into each word:

| method | s / generation | cells / s | cells correct |
|---|---|---|---|
| rule, CPU | 0.0780 | 5.4e7 | all 4,194,304 |
| lookup table, CPU | 0.0380 | 1.1e8 | all 4,194,304 |
| lookup table, GPU, read back | 0.0917 | 4.6e7 | all 4,194,304 |
| lookup table, GPU, kept there | 0.0016 | 2.7e9 | all 4,194,304 |
| bitwise, GPU | 8.37e-5 | 5.0e10 | all 4,194,304 |

The graphics processor wins once the grid stays on it: the lookup table kept on the GPU is about 49 times faster than the CPU rule, and the bitwise kernel about 930 times. Reading the board back after every generation costs more than the computation saves, and that row is slower than the CPU lookup table.
