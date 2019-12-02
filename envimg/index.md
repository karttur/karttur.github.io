---
layout: page
title: EnvironImagine
excerpt: "Real world quality control with environmental imagine."
image: std-trmm-3b43v7-precip_3B43_trmm_2001-2016_A
search_omit: true
---

Based on ideas and algorithm developments that I have done over the past decades for interpreting multi-spectral satellite images, I want to develop a new approach for interpreting spectral data, whether from multi-spectral images or hyperspectral spectrometers. The EnvironImagine blog is an archive of ideas, inforamtion and manuals allowing me to keep track of the different aspects I need to juggle in order to expand my small corporation into a business offering an app (online tool or for download) that would allow civic users to become imagery citizen scientists.

<ul class="post-list">
{% for post in site.categories.enviroimagine %}
<li><article><a href="{{ post.karttururl }}">{{ post.title }} {% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a>
  {% if post.abstract %} <span class="excerpt">{{ post.abstract | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}
</article></li>
{% endfor %}
</ul>
