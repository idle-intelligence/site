---
layout: default
title: sensors-web
repo: ""
hf: ""
demo: ""
original_model: ""
dataset: ""
perf_highlight: ""
what_is: A page that probes which device sensors a mobile browser exposes without a permission prompt.
runs: browser, native
license: ""
status: not yet published
blurb: >-
  A dependency-free page that probes every sensor and device-info API a
  browser exposes without a permission prompt, plus a std-only Rust dev
  server to capture readings from a phone. Finding: on Android, motion
  sensors, compass, and much of the device fingerprint are freely
  available with zero user consent; iOS gates everything.
---

{{ page.blurb }}
