---
layout: default
title: Home
---

<section class="space-y-6 border border-[#d8cab0] bg-[#fcf9f3] p-8">
  <div class="flex flex-col gap-6 md:flex-row md:items-start md:justify-between">
    <div class="space-y-4">
      <p class="text-xs uppercase tracking-widest text-[#7a6d56]">Quick introduction</p>
      <h1 class="text-4xl font-extrabold leading-tight text-[#2f3e9d] md:text-6xl">Hi, I’m Rudi.</h1>
      <p class="max-w-2xl text-sm text-[#5d503a]">
        Welcome to my homepage. This is a concise overview of what I’m working on and where to find more details.
        Visit the CV page for structured background information and the blog for chronological markdown notes.
      </p>
    </div>
    <img
      src="{{ '/assets/images/profile.jpg' | relative_url }}"
      alt="Profile picture of Rudi"
      class="h-24 w-24 shrink-0 rounded-full border border-[#d8cab0] object-cover md:h-28 md:w-28"
    />
  </div>
</section>

<section class="mt-10 grid gap-4 md:grid-cols-2">
  <article class="border border-[#d8cab0] bg-[#fcf7ef] p-5">
    <h2 class="text-xs uppercase tracking-widest text-[#7a6d56]">Currently working on professionally</h2>
    <p class="mt-3 text-sm text-[#5d503a]">
      I’m currently working as a Working Student Machine Learning Engineer at Fraunhofer IOF in Jena, focusing on
      computer vision, image understanding, and 3D reconstruction workflows for practical applications.
    </p>
  </article>
  <article class="border border-[#d8cab0] bg-[#fcf7ef] p-5">
    <h2 class="text-xs uppercase tracking-widest text-[#7a6d56]">Open source projects</h2>
    <p class="mt-3 text-sm text-[#5d503a]">
      I regularly build and share smaller coding projects and experiments on
      <a href="https://github.com/I-am-Rudi">GitHub</a>, mostly around scientific computing and machine learning.
    </p>
  </article>
</section>

<section id="projects" class="mt-10 space-y-4">
  <h2 class="text-xs uppercase tracking-widest text-[#7a6d56]">Recent entries</h2>
  <div class="grid gap-4 md:grid-cols-2">
    {% assign entries = site.projects | concat: site.posts %}
    {% assign entries = entries | sort: "date" | reverse %}
    {% for item in entries %}
      <article class="border border-[#d8cab0] bg-[#fcf7ef] p-5">
        <p class="text-xs uppercase tracking-widest text-[#7a6d56]">{{ item.date | date: "%Y-%m-%d" }}</p>
        <h3 class="mt-2 text-xl font-bold leading-snug">
          <a class="no-underline" href="{{ item.url | relative_url }}">{{ item.title }}</a>
        </h3>
        {% if item.excerpt %}
          <p class="mt-3 text-sm text-[#5d503a]">{{ item.excerpt | strip_html | truncate: 140 }}</p>
        {% endif %}
      </article>
    {% endfor %}
  </div>
</section>
