---
layout: default
title: Home
---

<section class="section">
  <div class="flex flex-col gap-6 md:flex-row md:items-start md:justify-between">
    <div class="space-y-4">
      <p class="text-xs uppercase tracking-widest text-[#7a6d56]">Quick introduction</p>
      <h1 class="text-4xl font-extrabold leading-tight text-[#2f3e9d] md:text-6xl">Hi, I’m Rudi.</h1>
      <p class="max-w-2xl text-sm text-[#5d503a]">
        Welcome to my homepage. I’m a physicist and part time machine learning engineer based in Jena, Germany.
      </p>
      <p class="max-w-2xl text-sm text-[#5d503a]">
        Visit the CV page for an overview of my education and experience.
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
  <article class="card">
    <h2 class="card-title text-xs uppercase tracking-widest text-[#7a6d56]">Currently</h2>
    <p class="mt-3 text-sm text-[#5d503a]">
      I am actively looking for a PhD position in the field of quantum gravity, fundamental physics, or machine learning for scientific applications.
    </p>
    <p class="mt-3 text-sm text-[#5d503a]">
      I have just completed my master’s degree at the Friedrich-Schiller-University in Jena with a focus on quantum and gravitational physics. Currently I am working as a machine learning engineer at the Fraunhofer Institute for Applied Optics and Precision Engineering (IOF) in Jena, where I focus on computer vision.
    </p>
  </article>
  <article class="card">
    <h2 class="card-title text-xs uppercase tracking-widest text-[#7a6d56]">Open source projects</h2>
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
      <article class="card">
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
