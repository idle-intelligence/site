---
layout: card
title: Hive
kind: code
task_group: Distributed inference
repo: idle-intelligence/hive-server
more_repos:
  - idle-intelligence/hive-client
hf: ""
demo: "https://trucs.ai/swarm/"
demo_pages: ""
original_model: ""
dataset: ""
perf_highlight: ""
card_proof: ""
used_on:
  - title: swarm
    url: "https://trucs.ai/swarm/"
posts:
  - title: "Claude and the Swarm"
    url: "https://trucs.ai/blog/claude-and-the-swarm"
what_is: A swarm of small language models running in browser tabs, with a hub that routes questions to them.
runs: browser, WASM, WebGPU, native
license: Apache-2.0
status: experiment
blurb: >-
  The Hive is a swarm of small language models running in people's browser
  tabs. Anyone can open the page, watch the swarm work in a live log, ask it a
  question, or join it as a drone that lends its tab to answer other people's
  questions. There is no large model behind it and no inference on the server:
  every answer is produced by the drones connected at that moment. The hub,
  [hive-server](https://github.com/idle-intelligence/hive-server), is a Rust
  WebSocket server that connects the drones, turns each question into tasks for
  them and broadcasts a public log of ids, routing and timings, never the
  words. A small classifier sorts each question, up to three drones write
  candidate answers and another drone picks the best. The page, the classifier
  and a command-line drone live in
  [hive-client](https://github.com/idle-intelligence/hive-client). Drones run
  the lean engine and choose WebGPU, CPU threads or a single thread by what
  the device can do.
---

{{ page.blurb }}
