---
title: Discover uni
layout: default
--- 


{% for hecos in  site.data.hecos | where: hecos.code = "100629" %}

 <h1>  {{ hecos.code }} </h1>
  <h2> {{ hecos.term }} </h2>
  <p> {{ hecos.definition }} </p>

{% endfor %}

