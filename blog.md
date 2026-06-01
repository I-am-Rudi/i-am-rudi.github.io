---
layout: default
title: Blog
permalink: /blog/
---

<section class="section">
  <div>
    <p class="text-xs uppercase tracking-widest text-[#7a6d56]">Chronological markdown posts</p>
    <h1 class="mt-1 text-4xl font-bold">Blog</h1>
    <p class="mt-2 text-sm text-[#5d503a]">
      Notes and updates rendered with clean, readable defaults inspired by Obsidian-style markdown presentation.
    </p>
  </div>

  <div class="space-y-4">
    {% for post in site.posts %}
      <article class="card-blog">
        <p class="text-xs uppercase tracking-widest text-[#7a6d56]">{{ post.date | date: "%Y-%m-%d" }}</p>
        <h2 class="mt-1 text-2xl font-bold leading-snug">
          <a class="no-underline" href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h2>
        {% if post.excerpt %}
          <p class="mt-3 text-sm text-[#5d503a]">{{ post.excerpt | strip_html | truncate: 220 }}</p>
        {% endif %}
      </article>
    {% endfor %}
  </div>
</section>
