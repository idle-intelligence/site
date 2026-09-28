---
layout: card
title: hive-ml-classifier
kind: code
task_group: Text classification
repo: idle-intelligence/hive-ml-classifier
hf: idle-intelligence/inference-at-home
demo: "https://trucs.ai/classifier/"
demo_pages: ""
original_model: ""
dataset: ""
perf_highlight: ""
what_is: A small BERT-mini classifier that routes chat messages into intent categories.
runs: browser, WASM
model_size: 11M params, 43MB
license: ""
status: maintained
blurb: >-
  A team of Claude agents generated training data and fine-tuned a 4-layer BERT-
  mini (11M params, 43MB) to route swarm chat input into four intents: swarm,
  weather, time, other. Runs client-side via Rust/WASM, no network round-trip.
  v3 hits 94.4% accuracy, 94.3% weighted F1.
---

{{ page.blurb }}
