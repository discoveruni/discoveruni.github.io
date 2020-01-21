---
title: Discover uni
layout: default
---

{% if site.data.hecos.date == {{ "now" | date: "%Y-%m-%d }} %}
  <h1>  {{ site.data.hecos.code }} </h1>
  <h2> {{ site.data.hecos.term }} </h2>
  <p> {{ site.data.hecos.definition }} </p>
  <br />
{% endif %}


{% for hecos in site.data.hecos %}
  <h1>  {{ hecos.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>
  <br />
{% endfor %}
