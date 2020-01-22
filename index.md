---
title: Discover uni
layout: default
--- 
{% assign todayscode = site.data.hecos.date %}
{{ todayscode }}
{% if site.data.hecos.date == [today | date: "%Y-%m-%d"] %}
{{ Hello }}
{% endif %}
{% assign hecoscodeoftheday = site.data.hecos | where: "date", today %}
{% for hecos in  site.data.hecos %}
 <h1>  {{ hecos.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>
{% endfor %}

