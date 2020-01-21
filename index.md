---
title: Discover uni
layout: default
--- 
{% assign today = site.time | date: "%Y-%m-%d" %}
{% if site.data.hecos.date == today  %}
  <h1>  {{ site.data.hecos.code }} </h1>
  <h2> {{ site.data.hecos.term }} </h2>
  <p> {{ site.data.hecos.definition }} </p>
{% endif %}
