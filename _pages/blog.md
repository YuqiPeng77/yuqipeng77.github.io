---
layout: archive
title: "Blog"
permalink: /blog/
author_profile: true
summary: "A collection of my notes, ideas, and reflections."
---

{% if page.summary %}
<div style="font-size: 16px; color: #666; margin-top: -10px; margin-bottom: 20px;">
  {{ page.summary }}
</div>
{% endif %}

{% for post in site.blog reversed %}

<h2 style="font-size: 32px; margin-bottom: 4px;">
  <a href="{{ post.redirect_to }}" target="_blank">{{ post.title }}</a>
</h2>

{% if post.summary %}
  <div style="font-size: 15px; color: #555; margin-top: 0; margin-bottom: 2px;">
    {{ post.summary }}
  </div>
{% endif %}

<div style="font-size: 14px; color: #888; margin-top: 0;">
  {{ post.date | date: "%B %d, %Y" }}
</div>


{% endfor %}
