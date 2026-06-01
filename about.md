---
layout: default
title: About
permalink: /about/
---

{% capture about_intro %}
I am a physicist and machine learning engineer based in Jena, focused on quantum and gravitational physics, computational methods, and practical AI systems.
{% endcapture %}
{% include profile-intro.html subtitle="About me" title="Kevin Rudolf Siebert" title_class="text-4xl font-bold text-[#2f3e9d]" content=about_intro image_src="/assets/images/profile.jpg" image_alt="Profile picture of Kevin Rudolf Siebert" content_class="space-y-3 max-w-2xl text-sm text-[#5d503a]" %}

{% capture focus_areas_content %}
- Machine learning for computer vision and 3D reconstruction
- Quantum field theory, general relativity, and quantum gravity
- Scientific computing with Python, Julia, and C++
{% endcapture %}

{% capture quick_links_content %}
- [Curriculum Vitae]({{ '/cv/' | relative_url }})
- [Blog]({{ '/blog/' | relative_url }})
- [kr.siebert@icloud.com](mailto:kr.siebert@icloud.com)
- [GitHub: I-am-Rudi](https://github.com/I-am-Rudi)
{% endcapture %}

{% capture about_cards %}
{% include card.html title="Focus areas" content=focus_areas_content %}
{% include card.html title="Quick links" content=quick_links_content %}
{% endcapture %}
{% include grid.html class="mt-10 grid gap-4 md:grid-cols-2" content=about_cards %}
