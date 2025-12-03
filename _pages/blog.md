---
layout: single
title: "Blog"
permalink: /blog/
author_profile: true
---

{% for post in site.blog reversed %}
### <a href="{{ post.redirect_to }}" target="_blank">{{ post.title }}</a>

<span style="color: #666; font-size: 0.9em;">
{{ post.date | date: "%B %d, %Y" }}
</span>

<br><br>
{% endfor %}
