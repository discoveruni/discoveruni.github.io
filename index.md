---
title: Discover uni
layout: default
--- 

{% assign todayscode == "today" %}
{{ todayscode }}
{% for hecos in  site.data.hecos %}
 almost sausage
 <h1>  {{ todayscode.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>
{% endfor %}

