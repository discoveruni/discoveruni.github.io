---
title: Discover uni
layout: default
--- 
{% assign todayscode = "today" | date: "%Y-%m-%d"  %}
{% if site.data.hecos.code == "100629" %}
It WORKS
{% endif %}

{% assign todayscode = "today" | date: "%Y-%m-%d"  %}
{% if site.data.hecos.date == " 2020-01-22 " %}
It also WORKS
{% endif %}

{% for hecos in  site.data.hecos | where: hecos.code == "100629" %}
 bacon {{ todayscode }} sausage and bacon sausage
 {% if hecos.code == "100629" %}
 <h1>  {{ hecos.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>
 {% endif %}
{% endfor %}

