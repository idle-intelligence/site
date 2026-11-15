---
layout: card
title: inference-at-home
kind: model
task_group: Text classification
repo: idle-intelligence/hive-ml-classifier
hf: idle-intelligence/inference-at-home
demo: "https://trucs.ai/classifier/"
demo_pages: ""
used_on:
  - title: classifier
    url: "https://trucs.ai/classifier/"
original_model: ""
original_author: ""
contribution: Trained by Idle Intelligence.
base_note: bert-mini architecture, base checkpoint not recorded
dataset: ""
perf_highlight: ""
what_is: The Hive's two message classifiers, a 64-cell topic grid and the first 4-class intent model, ready to run in the browser.
runs: browser, WASM
model_size: 11M params, 43MB
license: Apache-2.0
status: maintained
blurb: >-
  Two classifiers, each with its weights, config.json and tokenizer.
  swarm-8x8, the one the Hive uses now, puts a message in one of 64 topic cells
  (8 domains of 8 subjects) so answers can be filed and retrieved per cell: a
  bge-small-en-v1.5 fine-tune with int8 weights. intent, the first Hive
  classifier, is a bert-mini fine-tune with four labels (swarm, weather, time,
  other), still used by the classifier demo on trucs.ai.
---

{{ page.blurb }}
