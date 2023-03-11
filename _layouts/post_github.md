---
layout: post
---
{% assign repo_name = page.repo_name | site.repository %}
{% assign repo = site.github.public_repositories | where:'name', repo_name %}


{{ repo | jsonify }}


{{ content }}