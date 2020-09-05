---
title: "Hello Egghead"
layout: "base.njk"
templateEngineOverride: njk,md
---

This is a home page.

## From the Blog

{% for post in collections.post | randomPost -%}
<a href="{{ post.data.url }}">{{ post.data.title }}</a>
{%- endfor %}

## Articles

<ul>
{%- for article in collections.articles -%}
<li><a href="{{ article.url }}">{{ article.data.title }}</a></li>
{%- endfor -%}
</ul>
