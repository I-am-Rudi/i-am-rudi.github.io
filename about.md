---
layout: default
title: About
permalink: /about/
---

<section class="section">
  <div class="flex flex-col gap-6 md:flex-row md:items-center md:justify-between">
    <div class="space-y-3">
      <p class="text-xs uppercase tracking-widest text-[#7a6d56]">About me</p>
      <h1 class="text-4xl font-bold text-[#2f3e9d]">Kevin Rudolf Siebert</h1>
      <p class="max-w-2xl text-sm text-[#5d503a]">
        I am a physicist and machine learning engineer based in Jena, focused on quantum and gravitational physics,
        computational methods, and practical AI systems.
      </p>
    </div>
    <img
      src="{{ '/assets/images/profile.jpg' | relative_url }}"
      alt="Profile picture of Kevin Rudolf Siebert"
      class="h-24 w-24 shrink-0 rounded-full border border-[#d8cab0] object-cover md:h-28 md:w-28"
    />
  </div>

  <div class="grid gap-4 md:grid-cols-2">
    <article class="card">
      <h2 class="card-title text-xs uppercase tracking-widest text-[#7a6d56]">Focus areas</h2>
      <ul class="mt-3 list-disc pl-5 text-sm text-[#5d503a]">
        <li>Machine learning for computer vision and 3D reconstruction</li>
        <li>Quantum field theory, general relativity, and quantum gravity</li>
        <li>Scientific computing with Python, Julia, and C++</li>
      </ul>
    </article>
    <article class="card">
      <h2 class="card-title text-xs uppercase tracking-widest text-[#7a6d56]">Quick links</h2>
      <ul class="mt-3 space-y-2 text-sm text-[#5d503a]">
        <li><a href="{{ '/cv/' | relative_url }}">Curriculum Vitae</a></li>
        <li><a href="{{ '/blog/' | relative_url }}">Blog</a></li>
        <li><a href="mailto:kr.siebert@icloud.com">kr.siebert@icloud.com</a></li>
        <li><a href="https://github.com/I-am-Rudi">GitHub: I-am-Rudi</a></li>
      </ul>
    </article>
  </div>
</section>
