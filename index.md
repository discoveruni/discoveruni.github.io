---
title: Discover uni
layout: default
--- 
{% assign hecoscodeoftheday = site.data.hecos | where: "date", site.time %}
{% for hecos in hecoscodeoftheday %}
This one: {{ hecos.code }}
{% endfor %}
{% for hecos in site.data.hecos %}
  <h1>  {{ hecos.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>
{% endfor %}
