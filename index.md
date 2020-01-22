---
title: Discover uni
layout: default
--- 

{% assign sausage = site.date.hecos | where: "code", "100826" %}
{{ sausage }}

{% for hecos in sausage %}

 <h1>  {{ hecos.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>

{% endfor %}

