---
layout: card
title: stencil-life
kind: model
task_group: Cellular automata
repo: idle-intelligence/llm-life
hf: idle-intelligence/stencil-life
demo: ""
demo_pages: "https://idle-intelligence.github.io/llm-life/web/"
original_model: ""
original_author: ""
contribution: Trained from scratch by Idle Intelligence.
dataset: ""
perf_highlight: ""
what_is: The smallest from-scratch networks trained to reproduce Conway's Game of Life exactly.
runs: browser, WASM, WebGPU
model_size: 3 models, 1.4K-3.5K params each
license: MIT
status: maintained
blurb: >-
  Three from-scratch alternatives to the language-model approach in llm-life: a
  one-layer BERT-style encoder over the 9 neighborhood cells, a 2-layer MLP over
  the same 9 values, and a stencil-masked attention model that takes the whole
  grid in one pass. All three are exact on every one of the 512 possible
  neighborhoods; the stencil model's weights, trained only at 16x16, stay exact
  up to 256x256 because the mask encodes the rule, not the grid size.
---

{{ page.blurb }}
