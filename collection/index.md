---
layout: default
title: Collection
permalink: /collection/
---

# Collection

<p class="tagline">Repos, weights, and datasets that came out of the lab.</p>

{% for item in site.collection %}
<p class="section-label">{{ item.title }}</p>

{{ item.blurb }}

<ul>
  {% if item.repo and item.repo != "" %}<li>Repo: <a href="https://github.com/{{ item.repo }}">{{ item.repo }}</a></li>{% endif %}
  {% if item.hf and item.hf != "" %}<li>HuggingFace: <a href="https://huggingface.co/{{ item.hf }}">{{ item.hf }}</a></li>{% endif %}
  {% if item.demo and item.demo != "" %}<li>Demo: <a href="{{ item.demo }}">{{ item.demo }}</a></li>{% endif %}
  {% if item.original_model and item.original_model != "" %}<li>Original model: {{ item.original_model }}</li>{% endif %}
  {% if item.dataset and item.dataset != "" %}<li>Dataset: <a href="https://huggingface.co/datasets/{{ item.dataset }}">{{ item.dataset }}</a></li>{% endif %}
  {% if item.perf_highlight and item.perf_highlight != "" %}<li>Perf: {{ item.perf_highlight }}</li>{% endif %}
</ul>

<hr>
{% endfor %}

Go back [home]({{ '/' | relative_url }}).
