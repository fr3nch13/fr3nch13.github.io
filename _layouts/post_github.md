---
layout: post
---
{% if page.repo_name %}
    {% assign repos = site.github.public_repositories | where:'name', page.repo_name | null %}
    {% assign repo = repos[0] %}
{% endif %}

{% if repo %}
    {% include sidebar-repo.html %}
{% endif %}

{{ content }}