---
layout: card
title: sensors-web
kind: code
task_group: Sensor and privacy research
repo: ""
hf: ""
demo: ""
demo_pages: ""
original_model: ""
dataset: ""
perf_highlight: ""
card_proof: ""
what_is: A page that probes which device sensors a mobile browser exposes without a permission prompt.
runs: browser, native
license: ""
status: not yet published
blurb: >-
  A dependency-free page that probes every sensor and device-info API a browser
  exposes without a permission prompt, plus a std-only Rust dev server to
  capture readings from a phone. Finding: on Android, motion sensors, compass,
  and much of the device fingerprint are freely available with zero user
  consent; iOS gates everything.
---

{{ page.blurb }}
