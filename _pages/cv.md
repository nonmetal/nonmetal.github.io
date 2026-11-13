---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

[[Download Full CV (PDF)]](/files/JoonParkCV_full.pdf)

Education
======
* **Ph.D. Student**, The University of Tokyo, Apr. 2025 ~ Present
  * Department of Information Physics & Computing, Graduate School of Information Science and Technology
  * Research Theme: Towards emotional, expressive speech generation model based on linguistic analysis of speech token and automatic evaluation of acoustic signals
  * Advisor: Yuki Saito
* **Master's Degree**, The University of Tokyo, Apr. 2023 ~ Mar. 2025
  * Department of Electrical Engineering & Information Systems, Graduate School of Engineering
  * Thesis: A Study on Analysis of Discrete Speech Representation Using Self-Supervised Learning Model and its Application to Speech Synthesis
  * Advisor: Daisuke Saito / GPA: 3.0 / 3.0
* **Bachelor's Degree**, Sogang University, Mar. 2016 ~ Feb. 2022
  * Major in Artificial Intelligence, Department of Electronic Engineering, School of Engineering
  * Thesis: Development of an Interactive Voice User Interface in Kiosk System Using Deep Learning
  * Advisor: Hyung-Min Park / GPA: 3.54 / 4.3
  * Military Service Period: Nov. 2017 ~ Aug. 2019

Research Interests
======
* Speech Synthesis / Speech Language Model
* Speech Evaluation / MOS Prediction System
* Self-Supervised Learning Models / Neural Audio Codecs
* Post-training with Reinforcement Learning
* Generative models (Autoregressive, Diffusion model)

Work Experiences
======
* **Spellbrush** — Researcher (Part-time), Oct. 2025 ~ Oct. 2026
  * Research on speech generation in multimodal dialogue models and video generation models
* **Cygames Inc.** — Researcher (Part-time), Oct. 2024 ~ Jun. 2025
  * Research on real-time foley sound synthesis in the virtual environment
* **Preferred Networks Inc.** — Researcher (Internship), Aug. 2024 ~ Dec. 2024
  * Research on multilingual emotional speech synthesis with spherical vectors and discrete speech tokens
* **NTT R&D** — Researcher (Internship), Jan. 2024 ~ Feb. 2024
  * Analysis towards G2P-free speech synthesis using text-speech token encoder through hidden unit T5
* **DeNA Co., Ltd.** — AI Specialist (Internship), Aug. 2023 ~ Oct. 2023
  * Improvement and implementation of cross-lingual voice conversion for products
* **CoeFont Co., Ltd.** — Researcher (Part-time), Apr. 2023 ~ Mar. 2026
  * Improvement and acceleration of the self-supervised learning framework to create natural and real-time speech synthesis and voice conversion
* **Samsung Medical Center** — Research Assistant (Part-time), Sep. 2020 ~ Jun. 2021
  * Optimization of classification model and distillation of datasets for detecting diseases from cardiac MRI

Research Experiences
======
* **Music and Audio Computing Lab, KAIST** — Visiting Research Student, Jul. 2026 ~ Sep. 2026
  * Research on vocal coaching models, fake music detection, and speech neural audio codecs
* **LY Corporation** — Industry-Academic Collaborative Research, Apr. 2025 ~ Mar. 2026
  * Research on generating speech-to-face expression generation for virtual avatar
* **Darrell Group, University of California, Berkeley** — Visiting Research Student, Jun. 2024 ~ Jul. 2024
  * Research on analyzing the language of text-derived tokens from various modalities, including visual, auditory, and multimodal media
* **Saruwatari & Koyama Lab, The University of Tokyo** — Research Student, Apr. 2022 ~ Mar. 2023
  * Research on self-supervised learning and generative model on speech synthesis for post-filter signal processing used in speech enhancement
* **Intelligent Information Processing Lab, Sogang University** — Internship, Oct. 2021 ~ Mar. 2022
  * Development of dialogue system and speech synthesis in IIPERIA: Intelligent Information Processing with End-2-end Representation for Interactive Assistant
* **Auditory Intelligent Lab, Sogang University** — Internship, Jan. 2021 ~ Jun. 2021
  * Development of SGRecognizer Demo: Korean unlimited vocabulary speech recognition system using Kaldi

Honors and Scholarships
======
* **Japan Society for the Promotion of Science Doctoral Course Research Fellowships (JSPS DC2)**, Apr. 2026 ~ Mar. 2028
  * 225,000 JPY/month + Research Funds
* **Best Paper Award**, Sound Symposiums 2025, Jun. 2025
* **Best Student Paper Award (LY Corporation Award)**, 154th Conference on Spoken Language Processing (SLP), Dec. 2024
* **Japanese Government (MEXT) Scholarship**, Apr. 2022 ~ Mar. 2026
  * 147,000 JPY/month
* **Best Undergraduate Paper Award**, Korean Information Science Society, May 2021

Teaching and Educational Experience
======
* **Software II** — Teaching Assistant, Oct. 2023 ~ Jan. 2024
  * Course for second-year students, Department of Electronic and Information Engineering, Faculty of Engineering, The University of Tokyo

Other Projects & Experiences
======
* **jarre.ai** — Team Leader, Product Designer, AI Engineer, Jan. 2025 ~ Sep. 2025
  * Student-based startup project with the theme of "Text-based AI implementation solution tool for video games"
  * Selected project for the 2025 UTokyo Spring Founders Program

Skills
======
* **Technologies**
  * Libraries: PyTorch, Transformers, librosa etc.
  * Programming Languages: Python, C, MATLAB, shell etc.
  * Software Development Tools: Git, Docker, Jupyter, Codex etc.
* **Spoken Languages**
  * Korean (Native), English, Japanese (Near Native), Chinese (Fully Professional)

Publications
======
See the [Publications](/publications/) page for project pages, code and highlights.

{% for category in site.publication_category %}
  {% assign items = site.publications | where: "category", category[0] | sort: "date" | reverse %}
  {% if items.size > 0 %}
  <h3 class="pub-category">{{ category[1].title }}</h3>
  <ol class="pub-list">
    {% for pub in items %}
      {% include publication-list-item.html pub=pub %}
    {% endfor %}
  </ol>
  {% endif %}
{% endfor %}
