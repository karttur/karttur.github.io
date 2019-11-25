---
layout: page
title: Blog Setup
excerpt: "Blogs on how I setup, created, developed and launched my different blogs.
."
image: std-trmm-3b43v7-precip_3B43_trmm_2001-2016_A
search_omit: true
---

When I started my blogs back in 2017, I the first things I learnt were how to [Set up blog tools: Jekyll and Atom](https://karttur.github.io/setup-blog/2017/12/21/setup-blog-tools.html). The second blog I created was on [Setup GitHub pages](https://karttur.github.io/setup-github/index.html) and includes more details on how Jekyll works. I then searched for a Jekyll theme to use for all my blogs and finally selected [So Simple](https://github.com/mmistakes/so-simple-theme) by Michael Rose. Since I started with _So Simple_ it has gone through a major upgrade, but I still use the older version. Mainly because I customized it extensively to fit my needs as described in my blog on [Setup Jekyll Theme Blog](https://karttur.github.io/setup-theme-blog/).

<ul class="post-list">
{% for post in site.categories.blogblog %}
<li><article><a href="{{ post.karttururl }}">{{ post.title }} {% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a>
  {% if post.abstract %} <span class="excerpt">{{ post.abstract | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}
</article></li>
{% endfor %}
</ul>
