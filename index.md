---
layout: default
---

{%- assign recent = site.posts | slice: 0, 3 -%}
{%- assign latest20 = site.posts | slice: 0, 20 -%}

<section>
  <h2 style="margin-top:0;">Derniers articles</h2>
  {%- for post in recent -%}
  <article class="card">
    <h3 class="post-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <div class="post-meta">{{ post.date | date: site.minima.date_format }} · {{ post.categories | join: ", " }}</div>
    {%- if post.description -%}
      <p>{{ post.description }}</p>
    {%- else -%}
      <p>{{ post.excerpt | strip_html | truncate: 180 }}</p>
    {%- endif -%}
    <a class="btn" href="{{ post.url | relative_url }}">Lire</a>
  </article>
  {%- endfor -%}
</section>

<section>
  <h2>Les 20 derniers</h2>
  <ul>
    {%- for post in latest20 -%}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> <span class="post-meta">— {{ post.date | date: site.minima.date_format }}</span></li>
    {%- endfor -%}
  </ul>
</section>