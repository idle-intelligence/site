---
layout: card
title: ridgeline
kind: code
task_group: Terrain and visualization
repo: idle-intelligence/ridgeline
hf: ""
demo: ""
demo_pages: "https://idle-intelligence.github.io/ridgeline/web/"
original_model: ""
dataset: idle-intelligence/ridgeline-terrain
perf_highlight: ""
used_on:
  - title: astres
    url: "https://trucs.ai/astres/"
posts:
  - title: "About astres (ridgeline)"
    url: "https://trucs.ai/blog/about-astres"
what_is: A 3D globe visualizer that renders planetary terrain as stacked ridgeline plots.
runs: browser, WASM, WebGPU
license: MIT
status: maintained
blurb: >-
  3D WebGPU explorer of the solar system's solid worlds, each rendered as a
  globe of stacked Joy Division "Unknown Pleasures" latitude ridgelines from
  real elevation data. Eleven bodies, Rust/WASM heightfield core plus a WGSL
  compute pass. Terrain streams progressively from a Hugging Face dataset as the
  camera descends.
---

{{ page.blurb }}
