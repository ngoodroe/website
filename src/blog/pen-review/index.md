---
title: Pen Reviews
layout: base.njk
eleventyExcludeFromCollections: true
permalink: /blog/pen-reviews/
---

# {{ title }}

<ul>
{%- for post in collections.blog %}
{%- if post.url.startsWith('/blog/pen-review/') and post.url != '/blog/pen-review/' %}
  <li><a href="{{ post.url }}">{{ post.data.title }}</a> — {{ post.date | dateFormat }}</li>
{%- endif %}
{%- endfor %}
</ul>
