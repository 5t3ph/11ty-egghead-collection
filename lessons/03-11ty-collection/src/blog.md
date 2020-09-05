---
title: "Blog"
layout: "base.njk"
---

## All Posts

<ul>
{%- for post in collections.post -%}
<li><a href="{{ post.url }}">{{ post.data.title }}</a></li>
{%- endfor -%}
</ul>
