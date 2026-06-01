---
layout: default
title: CV
permalink: /cv/
---

{% capture cv_left_content %}
# Kevin Rudolf Siebert

_Curriculum Vitae_
{% endcapture %}

{% capture cv_right_content %}
Am Egelsee 10

07743 Jena

+49 151 0501030

kr.siebert@icloud.com
{% endcapture %}

{% capture cv_sections %}
{% include cv-heading.html padding_class="pt-2" title="Education" description="Grades in German grading system, where 1.0 is the best grade and 4.0 the lowest passing grade." %}

{% capture master_science_content %}
**Friedrich-Schiller-University, Jena, grade: 1.2.**

- Specialization: Gravitational and Quantum Physics
- Emphasis on Quantum Field Theory, General Relativity and Quantum Gravity
{% endcapture %}
{% include cv-item.html date="10/2021 – 12/2025" content=master_science_content %}

{% capture year_abroad_content %}
**University of Geneva (UNIGE), Geneva.**

- Emphasis on Quantum Field Theory and Quantum Information Theory
{% endcapture %}
{% include cv-item.html date="09/2022 – 07/2023" content=year_abroad_content %}

{% capture bachelor_science_content %}
**Friedrich-Schiller-University, Jena, grade: 1.8.**
{% endcapture %}
{% include cv-item.html date="10/2018 – 10/2021" content=bachelor_science_content %}

{% capture coursework_content %}
**Quantum Theory, QFT & GR**

Quantum Theory (1.0); Quantum Field Theory (1.7); Quantum Information Theory (1.7); Selected Topics in Quantum Information (1.0); Relativistic Physics (1.7); Current Topics in Gravitational and Quantum Theory II, III (1.0, 1.0)

**Mathematics & Computer Science**

Complex Analysis (2.0), Informatics I, II (1.0, 1.3); Computational Physics I, II (2.0) & IV (1.3); Machine Learning (2.0)
{% endcapture %}
{% include cv-item.html date="Relevant coursework" content=coursework_content %}

{% include cv-heading.html title="Master Thesis" %}

{% capture master_thesis_title %}
**Exploring Effective Spin Foams with Monte Carlo in SU(2) BF Theory**
{% endcapture %}
{% include cv-item.html date="Title" content=master_thesis_title %}

{% capture master_thesis_supervisors %}
Prof. Dr. Holger Gies & Dr. Sebastian Steinhaus
{% endcapture %}
{% include cv-item.html date="Supervisors" content=master_thesis_supervisors %}

{% capture master_thesis_grade %}
1.0
{% endcapture %}
{% include cv-item.html date="Grade" content=master_thesis_grade %}

{% capture master_thesis_description %}
- Studying contributions of discrete geometries to the state sum in the Ooguri model
- Investigating this topological field theory model as a toy model for full quantum gravitational state sums in the spin foam approach to quantum gravity
- Using Monte Carlo methods as a mathematical probe into these contributions
{% endcapture %}
{% include cv-item.html date="Description" content=master_thesis_description %}

{% include cv-heading.html title="Bachelor Thesis" %}

{% capture bachelor_thesis_title %}
**Bootstrapping Quantum Mechanical Systems**
{% endcapture %}
{% include cv-item.html date="Title" content=bachelor_thesis_title %}

{% capture bachelor_thesis_supervisors %}
Prof. Dr. Martin Ammon & Dr. Georg Bergner
{% endcapture %}
{% include cv-item.html date="Supervisors" content=bachelor_thesis_supervisors %}

{% capture bachelor_thesis_grade %}
1.5
{% endcapture %}
{% include cv-item.html date="Grade" content=bachelor_thesis_grade %}

{% capture bachelor_thesis_description %}
- Bootstrap method from conformal field theory applied to anharmonic oscillators
- Extensive comparison to established numerical methods
{% endcapture %}
{% include cv-item.html date="Description" content=bachelor_thesis_description %}

{% include cv-heading.html title="Experience" %}

{% capture ml_engineer_content %}
**Fraunhofer IOF, Jena.**

- Research and development of computer vision machine learning algorithms
- Main focus on image classification, detection and 3D-reconstruction
- Specialized models (2D/3D Gaussian Splatting and Neural Radiance Fields)
- Relevant workflow: convolutional neural networks and transformer networks with focus on shifted window transformers (Swin)
- Researched, developed and deployed an industry-grade deep learning pipeline on my own
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

{% capture physics_skills %}
Quantum Field Theory, General Relativity, Quantum Gravity, Quantum Information Theory, Computational Physics
{% endcapture %}
{% include cv-item.html date="Physics" content=physics_skills %}

{% capture math_skills %}
Group Theory and Representation Theory, Lie Algebras, Differential Geometry, Discrete Geometry, Complex Analysis, Algebraic Topology, Algebraic Geometry
{% endcapture %}
{% include cv-item.html date="Mathematics" content=math_skills %}

{% capture documentation_skills %}
LaTeX, TikZ, PGFplots, Mermaid
{% endcapture %}
{% include cv-item.html date="Documentation" content=documentation_skills %}

{% capture programming_skills %}
Julia, Python (numpy, matplotlib, pytorch, numba), C++
{% endcapture %}
{% include cv-item.html date="Programming" content=programming_skills %}

{% capture computer_algebra_skills %}
Wolfram language/Mathematica, SymPy
{% endcapture %}
{% include cv-item.html date="Computer Algebra" content=computer_algebra_skills %}

{% capture software_skills %}
Linux, Git, Inkscape, Obsidian
{% endcapture %}
{% include cv-item.html date="Software" content=software_skills %}
{% endcapture %}

{% include profile-intro.html content=cv_left_content right_content=cv_right_content content_class="space-y-2 text-[#5d503a]" right_class="text-sm cv-meta" %}
{% include stack.html class="mt-10 space-y-0" content=cv_sections %}
