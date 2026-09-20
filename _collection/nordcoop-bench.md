---
layout: default
title: nordcoop-bench
repo: ""
hf: ""
demo: ""
original_model: ""
dataset: ""
perf_highlight: "33.2 t/s decode (Qwen3-Next-80B-A3B Config A, RAM-resident), RTX 3080 10GB + Ryzen 9 3900X + 64GB DDR4-3000"
what_is: A reproducible benchmark comparing local language models against hosted references on constrained hardware.
runs: native
license: ""
status: experiment
blurb: >-
  A reproducible bench measuring what hardware buys what local-LLM regime
  for Claude-Code-style single-shot delegation tasks. Runs local MoE
  models on a constrained rig, scores them against Sonnet/Haiku/Opus
  references, and projects to bigger hardware via a bandwidth-bound
  scaling formula.
---

{{ page.blurb }}
