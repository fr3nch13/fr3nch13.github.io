---
layout: splash
author_profile: true
taxonomy: "personal"
title: Personal
permalink: /personal/
header:
  overlay_filter: {{ site.custom.hero_overlay }}
  overlay_image: /assets/images/banner-personal.jpg
excerpt: "Personal things I'd like to highlight."
date: ''
---

This will list out the different things in my personal life that I'd like to highlight.

## Posts

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% include posts-category.html taxonomy=page.taxonomy type=entries_layout %}
</div>