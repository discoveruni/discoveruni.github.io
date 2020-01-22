---
title: Discover uni
layout: default
--- 
{% if site.data.hecos.date == today %}
{{ Hello }}
{% endif %}
{% assign hecoscodeoftheday = site.data.hecos | where: "date", today %}
{% for hecos in hecoscodeoftheday %}
This one:
 <h1>  {{ hecos.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>
{% endfor %}

