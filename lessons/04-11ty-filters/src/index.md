---
title: "Hello Egghead"
layout: "base.njk"
templateEngineOverride: njk,md
---

This is a home page.

## From the Blog

{% for post in collections.post | randomPost -%}
<a href="{{ post.url }}">{{ post.data.title }}</a>
{%- endfor -%}
