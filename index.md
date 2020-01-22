---
title: Discover uni
layout: default
--- 
{% assign bacon = "today" | date: "%Y-%m-%d" %}
{{ bacon }}
{% assign sausage = site.data.hecos | where: "date", bacon %}
{{ sausage }}

{% for hecos in sausage %}

 <h1>  {{ hecos.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>

{% endfor %}

