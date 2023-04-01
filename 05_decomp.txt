---
layout: page
title: Decomp
permalink: /n64/
---

<ul>
{% for post in site.categories.Decompilation %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>