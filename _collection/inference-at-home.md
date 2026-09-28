---
layout: card
title: inference-at-home
kind: model
task_group: Text classification
repo: idle-intelligence/hive-ml-classifier
hf: idle-intelligence/inference-at-home
demo: "https://trucs.ai/classifier/"
demo_pages: ""
original_model: ""
dataset: ""
perf_highlight: ""
what_is: The trained weights behind hive-ml-classifier's swarm-intent BERT.
runs: browser, WASM
model_size: 11M params, 43MB
license: ""
status: maintained
blurb: >-
  Fine-tuned bert-mini weights (safetensors, config.json, tokenizer) for the
  4-class swarm-intent classifier used by hive-ml-classifier: swarm, weather,
  time, other. v3 hits 94.4% accuracy and 94.3% weighted F1 on held-out data.
---

{{ page.blurb }}
