---
title: Discover uni
layout: default
--- 
{{site.time | date: "%Y-%m-%d"}}
{% if site.data.hecos.date == site.time | date: "%Y-%m-%d"  %}
  <h1>  {{ site.data.hecos.code }} </h1>
  <h2> {{ site.data.hecos.term }} </h2>
  <p> {{ site.data.hecos.definition }} </p>
{% endif %}
