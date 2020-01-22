---
title: Discover uni
layout: default
--- 

{% for hecos in  site.data.hecos %}
{% assign todayscode == today | date: "%Y-%m-%d" %}
 <h1>  {{ todayscode.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>
{% endfor %}

