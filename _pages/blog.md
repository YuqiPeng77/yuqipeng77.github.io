---
layout: archive
title: "Blogs"
permalink: /blog/
author_profile: true
summary: "A collection of my notes, ideas, and reflections."
---

{% if page.summary %}
<div style="font-size: 0.9em; color: #555; margin-top: 6px; margin-bottom: 12px;">
{{ page.summary }}
</div>

  {{ page.summary }}
</div>
{% endif %}

{% comment %}
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
{% endcomment %}


{% for post in site.blog reversed %}

<h2 class="archive__item-title">
  <a href="{{ post.redirect_to }}" target="_blank">{{ post.title }}</a>
</h2>

{% if post.summary %}
  <p class="archive__item-excerpt">
    {{ post.summary }}
  </p>
{% endif %}

<p class="page__meta">
  {{ post.date | date: "%B %d, %Y" }}
</p>

{% endfor %}

