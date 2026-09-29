---
layout: card
title: weather-web
kind: code
task_group: Weather
repo: idle-intelligence/weather-web
hf: ""
dataset: idle-intelligence/metar-stations
demo: ""
demo_pages: "https://idle-intelligence.github.io/weather-web/web/"
original_model: ""
used_on:
  - title: weather
    url: "https://trucs.ai/knn-weather/"
posts:
  - title: "Browser weather"
    url: "https://trucs.ai/blog/browser-weather"
perf_highlight: ""
what_is: A weather estimate for any point on Earth from the nearest METAR-reporting stations.
runs: browser, WASM, native
license: MIT
status: maintained
blurb: >-
  The k nearest METAR stations within 100km are averaged by inverse distance
  weighting, with corrections for elevation (a lapse rate fitted across the
  neighbours), dew point (averaged as vapour pressure), pressure (averaged as
  sea-level QNH), and wind (averaged as vector components). The method comes
  from SenseAI's weather tools (2015); this crate is its Rust implementation and
  source of truth, running entirely client-side via WebAssembly.
---

{{ page.blurb }}
