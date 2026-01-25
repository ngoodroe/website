---
title: Blog
layout: base.njk
eleventyExcludeFromCollections: true
permalink: /blog/
---

# {{ title }}

<ul>
{%- for post in collections.blog %}
  <li><a href="{{ post.url }}">{{ post.data.title }}</a> 
  {%- if post.data.description %}
  — {{ post.data.description }}
  {%- endif %}
  </li>
{%- endfor %}
</ul>
