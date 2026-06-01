---
layout: default
title: Blog
permalink: /blog/
---

{% capture blog_intro %}
Notes and updates rendered with clean, readable defaults inspired by Obsidian-style markdown presentation.
{% endcapture %}
{% include profile-intro.html subtitle="Chronological markdown posts" title="Blog" content=blog_intro right_content="Markdown posts, notes, and experiments." %}

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
{% include stack.html class="mt-10 space-y-4" content=blog_posts %}
