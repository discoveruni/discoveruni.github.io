---
title: Discover uni
layout: default
--- 
{% assign todayscode == "today" | date: "%Y-%m-%d %}

{% for hecos in  site.data.hecos %}
{{ todayscode }}
 <h1>  {{ todayscode.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>
{% endfor %}

