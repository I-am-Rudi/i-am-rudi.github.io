---
layout: default
title: Blog
permalink: /blog/
---

{% capture blog_intro %}
This part of the website is for some thoughts that I want to
{% endcapture %}
{% include profile-intro.html subtitle="Markdown posts, notes, and experiments." title="Blog" content=blog_intro right_content="" right_below=true %}

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
