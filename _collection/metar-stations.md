---
layout: card
title: metar-stations
kind: dataset
task_group: Weather
repo: idle-intelligence/weather-web
hf: ""
dataset: idle-intelligence/metar-stations
demo: ""
demo_pages: ""
original_model: ""
original_author: ""
contribution: Built by Idle Intelligence from the Iowa Environmental Mesonet ASOS/AWOS network.
perf_highlight: ""
what_is: A worldwide roster of METAR/ASOS weather stations, sourced from the Iowa Environmental Mesonet.
runs: ""
license: CC0-1.0
status: maintained, updated weekly
blurb: >-
  A worldwide roster of METAR/ASOS stations across the IEM ASOS/AWOS networks,
  one network per country or US state/Canadian province. Stations that reported
  at least once in the trailing 7-day build window are in stations.json; silent
  stations are kept, flagged, in stations_all.json. Backs weather-web's
  nearest-station search. Published on Hugging Face. A scheduled Hugging Face Job
  rebuilds the roster every Monday, so the active list follows the stations
  that are actually reporting.
---

{{ page.blurb }}
