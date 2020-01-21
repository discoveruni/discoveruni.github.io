---
title: Discover uni
layout: default
--- 

{% if site.data.hecos.date == site.time  %}
  <h1>  {{ site.data.hecos.code }} </h1>
  <h2> {{ site.data.hecos.term }} </h2>
  <p> {{ site.data.hecos.definition }} </p>
{% endif %}
