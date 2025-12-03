---
layout: single
title: "Blog"
permalink: /blog/
author_profile: true
---

{% for post in site.blog reversed %}
<h2 style="font-size: 32px; margin-bottom: 0;">
  <a href="{{ post.redirect_to }}" target="_blank">{{ post.title }}</a>
</h2>

<p style="margin-top: 5px;">{{ post.date | date: "%B %d, %Y" }}</p>
{% endfor %}
