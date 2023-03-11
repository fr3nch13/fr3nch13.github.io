---
layout: post
---
{% assign repo_name = page.repo_name | site.repository %}
{% assign page.repo = site.github.public_repositories | where:'name', repo_name %}

{% if page.repo %}
{% include sidebar-repo.html %}
{% endif %}

<pre>
{{ page.repo | jsonify }}
</pre>

{{ content }}