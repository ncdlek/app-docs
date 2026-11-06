---
title: "Apps by Engin Yazılan — Capture GO and Game Clock Pro"
description: "iPhone and iPad apps for board game players by independent developer Engin Yazılan: Capture GO, a free way to learn Go, and Game Clock Pro, a byo-yomi and Fischer game clock."
kind: site
heading: Apps by Engin Yazılan
---

Small, careful iPhone and iPad apps for people who play board games — made by
one independent developer who plays Go.

<div class="apps">
{%- for entry in site.data.apps %}
{%- assign app = entry[1] %}
  <a class="app-card" href="{{ '/' | append: entry[0] | append: '/' | relative_url }}">
    <img src="{{ app.icon | relative_url }}" alt="" width="72" height="72">
    <div>
      <h2>{{ app.name }}</h2>
      <p>{{ app.tagline }}</p>
      <p class="small">{{ app.price_label }} · {{ app.platforms }}</p>
    </div>
  </a>
{%- endfor %}
</div>

Every app has an overview, a support page with answers to common questions, a
privacy policy and terms. For a plain-text summary of all apps, see
[llms.txt]({{ '/llms.txt' | relative_url }}).
