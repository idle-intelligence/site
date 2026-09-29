---
layout: card
title: hive-ml-classifier
kind: code
task_group: Text classification
repo: idle-intelligence/hive-ml-classifier
hf: idle-intelligence/inference-at-home
demo: ""
demo_pages: ""
original_model: ""
dataset: ""
perf_highlight: ""
used_on:
  - title: classifier
    url: "https://trucs.ai/classifier/"
  - title: swarm
    url: "https://trucs.ai/swarm/"
posts:
  - title: "Claude and the Swarm"
    url: "https://trucs.ai/blog/claude-and-the-swarm"
  - title: "Claude and the Swarm: the ML team"
    url: "https://trucs.ai/blog/claude-and-the-swarm-1-ml-team"
  - title: "Claude and the Swarm: the hive team"
    url: "https://trucs.ai/blog/claude-and-the-swarm-2-hive-team"
  - title: "Claude and the Swarm: the review team"
    url: "https://trucs.ai/blog/claude-and-the-swarm-3-review-team"
  - title: "Claude and the Swarm: more doc than code"
    url: "https://trucs.ai/blog/claude-and-the-swarm-4-more-docs-than-code"
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
