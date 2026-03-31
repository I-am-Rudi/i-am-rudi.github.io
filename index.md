---
layout: default
title: Home
---

<section class="space-y-6 border border-zinc-800 p-8">
  <p class="text-xs uppercase tracking-widest text-zinc-400">Developer Interface</p>
  <h1 class="text-5xl font-extrabold leading-tight md:text-7xl">BRUTALIST<br />PORTFOLIO</h1>
  <p class="max-w-2xl text-sm uppercase tracking-widest text-zinc-300">Monospaced by design. Minimal surface area. Maximum signal.</p>
</section>

<section id="projects" class="mt-10 space-y-4">
  <h2 class="text-xs uppercase tracking-widest text-zinc-400">Project Grid</h2>
  <div class="grid gap-4 md:grid-cols-2">
    {% assign entries = site.projects | concat: site.posts %}
    {% for item in entries %}
      <article class="border border-zinc-800 p-5">
        <p class="text-xs uppercase tracking-widest text-zinc-500">{{ item.date | date: "%Y-%m-%d" }}</p>
        <h3 class="mt-2 text-xl font-bold">
          <a class="no-underline" href="{{ item.url | relative_url }}">{{ item.title }}</a>
        </h3>
        {% if item.excerpt %}
          <p class="mt-3 text-sm text-zinc-300">{{ item.excerpt | strip_html | truncate: 140 }}</p>
        {% endif %}
      </article>
    {% endfor %}
  </div>
</section>
