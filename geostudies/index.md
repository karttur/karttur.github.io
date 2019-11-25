---
layout: page
title: Geo Studies
excerpt: "Geographical studies"
image: std-trmm-3b43v7-precip_3B43_trmm_2001-2016_A
search_omit: true
---

Geographical studies

<ul class="post-list">
{% for post in site.categories.geostudies %}
<li><article><a href="{{ post.karttururl }}">{{ post.title }} {% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a>
  {% if post.abstract %} <span class="excerpt">{{ post.abstract | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}
</article></li>
{% endfor %}
</ul>
