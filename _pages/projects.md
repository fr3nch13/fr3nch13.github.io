---
layout: splash
author_profile: true
taxonomy: "projects"
title: Projects
permalink: /projects/
header:
  overlay_filter: "linear-gradient(to bottom, #02b7ffbb, #02b7ff66)"
  overlay_image: /assets/images/banner-projects.jpg
excerpt: "Highlighted Projects I'm working on."
date: ''
---

This will list out the different projects I have.

## Posts

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% include posts-category.html taxonomy=page.taxonomy type=entries_layout %}
</div>