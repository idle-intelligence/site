---
layout: card
title: llm-of-life-lora
kind: model
task_group: Cellular automata
repo: idle-intelligence/llm-life
hf: idle-intelligence/llm-of-life-lora
demo: ""
demo_pages: "https://idle-intelligence.github.io/llm-life/web/"
original_model: Qwen/Qwen2.5-0.5B-Instruct
dataset: ""
perf_highlight: ""
what_is: LoRA adapters that turn Qwen2.5-0.5B-Instruct into a Game of Life update rule.
runs: browser, WASM, WebGPU
model_size: 4 adapters, ~1.1M params each, 4.1MB each
license: Apache-2.0
status: maintained
blurb: >-
  Four rank-8 LoRA adapters on Qwen2.5-0.5B-Instruct Q4_0 for llm-life: two read
  one cell's 3x3 neighborhood per forward pass (with and without the rules
  stated in the prompt), two read a whole 16x16 or 32x32 grid in one forward
  pass. The untrained base model gets 215 of 512 neighborhoods right with the
  rules stated; the trained adapters reach 509-512 of 512.
---

{{ page.blurb }}
