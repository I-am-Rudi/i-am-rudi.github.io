---
layout: default
title: Home
---

{% capture intro_content %}
Welcome to my homepage. I’m a physicist and part time machine learning engineer based in Jena, Germany.

Visit the CV page for an overview of my education and experience.
{% endcapture %}


{% include profile-intro.html subtitle="Quick introduction" title="Hi, I’m Rudi." content=intro_content image_src="/assets/images/profile.jpg" image_alt="Profile picture of Rudi" image_class="h-24 w-24 shrink-0 rounded-full border border-[#d8cab0] object-cover md:h-28 md:w-28 md:self-center md:-ml-3" %}

{% capture currently_content %}
- I am actively looking for a PhD position in the field of quantum gravity,
  fundamental physics, or machine learning for scientific applications.
- I have just completed my master’s degree at the Friedrich-Schiller-University in Jena with a focus on quantum and gravitational physics. 
- Currently, I am working as a machine learning engineer at the Fraunhofer Institute for Applied Optics and Precision Engineering (IOF) in Jena, where I focus on computer vision.
{% endcapture %}

{% capture projects_content %}
I regularly build and share smaller coding projects and experiments on [GitHub](https://github.com/I-am-Rudi), mostly around scientific computing and machine learning.
{% endcapture %}

{% capture home_cards %}
{% include card.html title="Currently" content=currently_content %}
{% include card.html title="Open source projects" content=projects_content %}
{% endcapture %}
{% include grid.html class="mt-10 grid gap-4 md:grid-cols-2" content=home_cards %}

{% include eyebrow.html text="Recent entries" %}
{% assign entries = site.projects | concat: site.posts %}
{% assign entries = entries | sort: "date" | reverse %}
{% capture recent_entries %}
{% for item in entries %}
{% capture entry_content %}
{{ item.date | date: "%Y-%m-%d" }}

### [{{ item.title }}]({{ item.url | relative_url }})
{% if item.excerpt %}
{{ item.excerpt | strip_html | truncate: 140 }}
{% endif %}
{% endcapture %}
{% include card.html content=entry_content %}
{% endfor %}
{% endcapture %}
{% include grid.html class="mt-4 grid gap-4 md:grid-cols-2" content=recent_entries %}
