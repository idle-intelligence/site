---
layout: card
title: agent-web
kind: code
task_group: LLM and tool calling
repo: idle-intelligence/agent-web
hf: ""
demo: ""
demo_pages: ""
original_model: Qwen/Qwen2.5-3B-Instruct
dataset: ""
perf_highlight: ""
card_proof: "3 of 33 eval cases solved"
what_is: A tool-calling agent loop for Qwen2.5-Instruct models, running on the lean inference engine.
runs: browser, WASM, WebGPU, native
model_size: 3B params (Q4_0 GGUF)
license: "model licence Apache-2.0; code licence MIT"
status: experiment
blurb: >-
  lean runs the model, text in and text out, on a backend it
  picks by capability. This repository holds what an agent adds on top: it
  renders each step's prompt with the model's own chat template and the tools,
  parses the model's tool calls out of its raw output, regenerates when a reply
  is malformed, calls an unknown tool or repeats a call, and repeats until the
  model gives a final text answer. It also holds an offline eval harness that
  scores runs against 46 utterance cases for a Sonos speaker-control tool set.
  With a 13-tool subset, 33 of the cases are solvable; Qwen2.5-3B-Instruct
  Q4_0 on the CPU with unconstrained decoding solved 3 of them (9.1%). The
  loop reaches the model through one small trait, so any engine that completes
  text can drive it. A wasm package runs the agent in a Web Worker.
---

{{ page.blurb }}
