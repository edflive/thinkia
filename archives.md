---
layout: default
title: Archives
permalink: /archives/
---

<h2>Les 20 derniers articles</h2>
<ul>
{%- assign latest20 = site.posts | slice: 0, 20 -%}
{%- for post in latest20 -%}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> <span class="post-meta">— {{ post.date | date: site.minima.date_format }}</span></li>
{%- endfor -%}
</ul>