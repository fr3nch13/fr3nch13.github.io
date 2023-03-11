---
layout: splash
author_profile: true
taxonomy: "projects"
title: Projects
permalink: /projects/
header:
  overlay_filter: { site.custom.hero_overlay }
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