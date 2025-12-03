---
layout: single
title: "Blog"
permalink: /blog/
author_profile: true
---

<h2>Blog Links</h2>

<ul>
{% for item in site.data.blog %}
  <li>
    <a href="{{ item.url }}" target="_blank">{{ item.title }}</a>
  </li>
{% endfor %}
</ul>
