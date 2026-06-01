---
layout: default
title: Blog
permalink: /blog/
---

{% include section-header.html subtitle="Chronological markdown posts" title="Blog" description="Notes and updates rendered with clean, readable defaults inspired by Obsidian-style markdown presentation." %}

{% capture blog_posts %}
{% for post in site.posts %}
{% capture post_content %}
{{ post.date | date: "%Y-%m-%d" }}

## [{{ post.title }}]({{ post.url | relative_url }})
{% if post.excerpt %}
{{ post.excerpt | strip_html | truncate: 220 }}
{% endif %}
{% endcapture %}
{% include card.html variant="card-blog" content=post_content %}
{% endfor %}
{% endcapture %}
{% include stack.html content=blog_posts %}
