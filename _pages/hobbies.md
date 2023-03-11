---
layout: splash
author_profile: true
taxonomy: "hobbies"
title: Hobbies
permalink: /hobbies/
header:
  overlay_filter: "linear-gradient(to bottom, #02b7ffbb, #02b7ff66)"
  overlay_image: /assets/images/banner-hobbies.jpg
excerpt: "Different hobbies I enjoy."
date: ''
---

This will list out the different hobbies I have.

## Posts

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% include posts-category.html taxonomy=page.taxonomy type=entries_layout %}
</div>