---
layout: post
---
{% assign repo_name = page.repo_name | site.repository | nil %}
{% if repo_name %}
    {% assign repo = site.github.public_repositories | where:'name', repo_name %}
{% endif %}

{% if repo %}
    {% include sidebar-repo.html %}
{% endif %}

<pre>
{{ repo | jsonify }}
</pre>

{{ content }}