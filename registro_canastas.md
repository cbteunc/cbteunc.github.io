---
layout: default
title: "Registro de CBTE"
---
<h1>{{ page.title }}</h1>

<table>
  <thead>
    <tr>
      <th>Fecha</th>
      <th>Título</th>
    </tr>
  </thead>
  <tbody>
    {% for post in site.posts %}
      {% if post.tags contains "canasta" %}
        <tr>
          <td>{{ post.date | date: "%d - %m - %Y" }}</td>
          <td><a href="{{ post.url }}">{{ post.title }}</a></td>
        </tr>
      {% endif %}
    {% endfor %}
  </tbody>
</table>

<a href="./index.html" class="btn-home">
    <i class="fa fa-long-arrow-left"></i> Volver al inicio
</a>