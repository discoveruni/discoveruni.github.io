---
title: Discover uni
layout: default
--- 
{% assign todayscode = "today" | date: "%Y-%m-%d"  %}
{% if site.data.hecos.date == todayscode %}
It WORKS
{% endif %}

{% assign todayscode = "today" | date: "%Y-%m-%d"  %}
{% if site.data.hecos.date == " 2020-01-22 " %}
It WORKS
{% endif %}

{% for hecos in  site.data.hecos  %}
 bacon {{ todayscode }} sausage and more sausage
 <h1>  {{ hecos.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>
{% endfor %}

