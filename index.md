---
layout: default
title: Home
---

<section class="space-y-6 border border-[#cfbfa1] bg-[#fbf7ef] p-8">
  <p class="text-xs uppercase tracking-widest text-[#7a6d56]">Quick introduction</p>
  <h1 class="text-4xl font-extrabold leading-tight md:text-6xl">Hi, I’m Rudi.</h1>
  <p class="max-w-2xl text-sm text-[#5d503a]">
    Welcome to my homepage. This is a concise overview of what I’m working on and where to find more details.
    Visit the CV page for structured background information and the blog for chronological markdown notes.
  </p>
</section>

<section id="projects" class="mt-10 space-y-4">
  <h2 class="text-xs uppercase tracking-widest text-[#7a6d56]">Recent entries</h2>
  <div class="grid gap-4 md:grid-cols-2">
    {% assign entries = site.projects | concat: site.posts %}
    {% assign entries = entries | sort: "date" | reverse %}
    {% for item in entries %}
      <article class="border border-[#cfbfa1] bg-[#f9f3e7] p-5">
        <p class="text-xs uppercase tracking-widest text-[#7a6d56]">{{ item.date | date: "%Y-%m-%d" }}</p>
        <h3 class="mt-2 text-xl font-bold">
          <a class="no-underline" href="{{ item.url | relative_url }}">{{ item.title }}</a>
        </h3>
        {% if item.excerpt %}
          <p class="mt-3 text-sm text-[#5d503a]">{{ item.excerpt | strip_html | truncate: 140 }}</p>
        {% endif %}
      </article>
    {% endfor %}
  </div>
</section>
