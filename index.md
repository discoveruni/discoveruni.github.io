---
title: Discover uni
layout: default
--- #
{% assign today = site.time | "%Y-%m-%d" %}
{% assign hecoscodeoftheday = site.data.hecos | where: "date", today %}
{% for hecos in hecoscodeoftheday %}
This one: {{ hecos.code }}
{% endfor %}
{% for hecos in site.data.hecos %}
  <h1>  {{ hecos.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>
{% endfor %}
