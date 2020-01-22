---
title: Discover uni
layout: default
--- 
{% assign todayscode = "today" | date: "%Y-%m-%d"  %}
 {{ "today" | date: "%Y-%m-%d" }}
{{ todayscode }}
{% for hecos in  site.data.hecos | where: hecos.date == todayscode %}
 bacon {{ todayscode }} sausage
 <h1>  {{ hecos.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>
{% endfor %}

