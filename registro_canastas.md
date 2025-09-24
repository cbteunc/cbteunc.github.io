---
layout: default
title: "Registro de CBTE"
---
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

<a href="./index.html" class="btn-home">
    <i class="fa fa-long-arrow-left"></i> Volver al inicio
</a>