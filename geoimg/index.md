---
layout: page
title: GeoImagine
excerpt: "Blogs on how I setup, created, developed and launched my different blogs.
."
image: std-trmm-3b43v7-precip_3B43_trmm_2001-2016_A
search_omit: true
---

Karttur's GeoImagine Framework is a Spatial Data Integrated development Environment (SPIDE) that can be used to _script your own Earth_. It is a toolbox for advanced handling of spatial data. To use the Framework you first have to [Install and setup spatial data IDE](https://karttur.github.io/setup-ide/) and then you can jump into [Karttur's GeoImagine Framework](https://karttur.github.io/geoimagine/).

<ul class="post-list">
{% for post in site.categories.geoimagine %}
<li><article><a href="{{ post.karttururl }}">{{ post.title }} {% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a>
  {% if post.abstract %} <span class="excerpt">{{ post.abstract | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}
</article></li>
{% endfor %}
</ul>
