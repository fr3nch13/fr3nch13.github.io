---
layout: post
---
{% if page.repo_name %}
    {% assign repo = site.github.public_repositories | where:'name', page.repo_name | first %}
{% endif %}

{{ content }}