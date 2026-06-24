---
layout: default
title: About
permalink: /about/
---

{% capture about_intro %}
I am a physicist and machine learning engineer based in Jena, focused on quantum and gravitational physics, computational methods, and practical AI systems.
{% endcapture %}
{% include profile-intro.html subtitle="About me" title="Kevin Rudolf Siebert" content=about_intro image_src="/assets/images/profile.jpg" image_alt="Profile picture of Kevin Rudolf Siebert" image_class="h-24 w-24 shrink-0 rounded-full border border-[#d8cab0] object-cover mt-8 md:mt-0 md:h-28 md:w-28 md:self-center md:-ml-3" %}

{% capture focus_areas_content %}
- Quantum field theory, general relativity, and quantum gravity
- Scientific computing with Python, Julia, and C++
- Machine learning applied to problems in physics
{% endcapture %}

{% capture quick_links_content %}
- [Curriculum Vitae]({{ '/cv/' | relative_url }})
- [Blog]({{ '/blog/' | relative_url }})
- [E-Mail](mailto:k.r.siebert@icloud.com)
- [GitHub: I-am-Rudi](https://github.com/I-am-Rudi)
{% endcapture %}

{% capture about_cards %}
{% include card.html title="Focus areas" content=focus_areas_content %}
{% include card.html title="Quick links" content=quick_links_content %}
{% endcapture %}
{% include grid.html class="mt-10 grid gap-4 md:grid-cols-2" content=about_cards %}
