---
layout: post
---
{% if page.repo_name %}
    {% assign repo = site.github.public_repositories | where:'name', page.repo_name | null %}
{% endif %}

{% if repo %}
    {% include sidebar-repo.html %}
{% endif %}

<pre>
{{ page.repo_name | jsonify }}
{{ repo | jsonify }}
</pre>

{{ content }}