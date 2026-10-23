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
card_proof: "94.4% accuracy, 94.3% F1"
used_on:
  - title: classifier
    url: "https://trucs.ai/classifier/"
  - title: swarm
    url: "https://trucs.ai/swarm/"
posts:
  - title: "Claude and the Swarm"
    url: "https://trucs.ai/blog/claude-and-the-swarm"
what_is: A small BERT-mini classifier that routes chat messages into intent categories, with a topic-grid successor in progress.
runs: browser, WASM
model_size: 11M params, 43MB
license: ""
status: v3 released, 8x8 successor in progress
blurb: >-
  A team of Claude agents generated training data and fine-tuned a 4-layer BERT-
  mini (11M params, 43MB) to route swarm chat input into four intents: swarm,
  weather, time, other. Runs client-side via Rust/WASM, no network round-trip.
  The released model, v3, reaches 94.4% accuracy and 94.3% weighted F1 on
  held-out data. A successor is in progress: a classifier that files each
  question into one of 64 topic cells on an 8x8 grid, so that the swarm can
  retrieve what it knows on that topic. Its test set of 4,000 real questions is
  labelled; the model is not trained yet.
---

{{ page.blurb }}
