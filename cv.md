---
layout: default
title: CV
permalink: /cv/
---

{% capture cv_right_content %}
[Github](https://github.com/I-am-Rudi)

[E-Mail](mailto:k.r.siebert@icloud.com)
{% endcapture %}

{% capture cv_sections %}
{% include cv-heading.html padding_class="pt-2" title="Education"%}

{% capture master_science_content %}
**Friedrich-Schiller-University, Jena.**

- Emphasis on Quantum Field Theory, General Relativity and Quantum Gravity
{% endcapture %}
{% include cv-item.html date="10/2021 – 12/2025" content=master_science_content %}

{% capture year_abroad_content %}
**University of Geneva (UNIGE), Geneva.**

- Emphasis on Quantum Field Theory and Quantum Information Theory
{% endcapture %}
{% include cv-item.html date="09/2022 – 07/2023" content=year_abroad_content %}

{% capture bachelor_science_content %}
**Friedrich-Schiller-University, Jena.**
{% endcapture %}
{% include cv-item.html date="10/2018 – 10/2021" content=bachelor_science_content %}

{% include cv-heading.html title="Master Thesis" %}

{% capture master_thesis_title %}
**Exploring Effective Spin Foams with Monte Carlo in SU(2) BF Theory**
{% endcapture %}
{% include cv-item.html date="Title" content=master_thesis_title %}

{% capture master_thesis_supervisors %}
Prof. Dr. Holger Gies & Dr. Sebastian Steinhaus
{% endcapture %}
{% include cv-item.html date="Supervisors" content=master_thesis_supervisors %}

{% include cv-heading.html title="Bachelor Thesis" %}

{% capture bachelor_thesis_title %}
**Bootstrapping Quantum Mechanical Systems**
{% endcapture %}
{% include cv-item.html date="Title" content=bachelor_thesis_title %}

{% capture bachelor_thesis_supervisors %}
Prof. Dr. Martin Ammon & Dr. Georg Bergner
{% endcapture %}
{% include cv-item.html date="Supervisors" content=bachelor_thesis_supervisors %}

{% include cv-heading.html title="Experience" %}

{% capture ml_engineer_content %}
**Fraunhofer IOF, Jena.**

- Research and development of computer vision machine learning algorithms
- Main focus on image classification, detection and 3D-reconstruction
{% endcapture %}
{% include cv-item.html date="11/2023 – today" content=ml_engineer_content %}

{% capture scientific_assistant_content %}
**Friedrich-Schiller-University, Jena.**

- Correction of exercise sheets for the lecture "Theoretical Electrodynamics" by Prof. Dr. Reinhard Meinel
{% endcapture %}
{% include cv-item.html date='04/2022 – 09/2022' content=scientific_assistant_content %}

{% capture student_assistant_content %}
**Friedrich-Schiller-University, Jena.**

- Correction of exercise sheets for the lecture "Thermodynamics and Statistical Mechanics" by Prof. Dr. Reinhard Meinel
{% endcapture %}
{% include cv-item.html date='10/2021 – 02/2022' content=student_assistant_content %}

{% capture tutoring_content %}
**Schülerhilfe Nachhilfe Cornelia Rosenberg, Jena.**

- Tutoring in mathematics and physics for high school students
{% endcapture %}
{% include cv-item.html date='09/2019 – 02/2021' content=tutoring_content %}

{% include cv-heading.html title="Key Skills" %}

{% capture documentation_skills %}
LaTeX, TikZ, PGFplots, Mermaid
{% endcapture %}
{% include cv-item.html date="Documentation" content=documentation_skills %}

{% capture programming_skills %}
Julia, Python, C++, C, JavaScript, Typescript
{% endcapture %}
{% include cv-item.html date="Programming" content=programming_skills %}

{% capture computer_algebra_skills %}
Wolfram language/Mathematica, SymPy
{% endcapture %}
{% include cv-item.html date="Computer Algebra" content=computer_algebra_skills %}

{% capture software_skills %}
Linux, Git, Docker, Inkscape, Obsidian, Vim/NeoVim, Visual Studio Code
{% endcapture %}
{% include cv-item.html date="Software" content=software_skills %}
{% endcapture %}

{% include profile-intro.html subtitle="Curriculum Vitae" title="Kevin Rudolf Siebert" right_content=cv_right_content content_class="space-y-2 text-[#5d503a]" right_class="text-sm cv-meta md:pt-10 md:-ml-6" right_style="margin-left:-1.5rem;" %}
{% include card-shell.html class="mt-10" content=cv_sections %}
