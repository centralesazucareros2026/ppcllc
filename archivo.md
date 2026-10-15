---
layout: default
title: Archivo
permalink: /archivo/
---
<h1>Archivo de artículos</h1>
<p>Todos los artículos publicados, del más reciente al más antiguo.</p>
<ul class="archive-list">
{% assign posts = site.posts %}
{% for post in posts %}
  <li><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%d/%m/%Y" }}</time><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></li>
{% endfor %}
</ul>
