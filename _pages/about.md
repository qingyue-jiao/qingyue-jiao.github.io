---
title: "About me"
permalink: /
excerpt: "Qingyue Jiao is a Ph.D. candidate at Notre Dame working on AI agents, multimodal memory, and reliable decision-making."
---

I am a third-year Ph.D. candidate in **Computer Science and Engineering at the University of Notre Dame**, advised by **[Prof. Yiyu Shi](https://cse.nd.edu/faculty/yiyu-shi/)**. Previously, I earned my M.S. in Computer Science from Columbia University and my B.S. in Computer Science and Physics from the University of Michigan.

My research focuses on helping **AI agents remember, reason, and make reliable decisions**. I work on multimodal memory architectures, memory evaluation, and decision-making under uncertainty, with the goal of improving evidence-grounded reasoning across multi-turn tasks.

<div class="availability"><strong>Open to internship opportunities.</strong> I am seeking research or engineering internships in AI agents, multimodal learning, and large language models. I welcome research collaborations—please <a href="mailto:qjiao@nd.edu">get in touch</a>.</div>

## Research interests

- **Multimodal agent memory:** preserving visual details, tracking updates, and retrieving the right evidence.
- **Reliable agent decision-making:** deciding when to clarify, search, act, or escalate under uncertainty.
- **Memory architectures and RAG:** organizing long, noisy contexts for accurate, evidence-grounded generation.

<p class="section-more"><a href="{{ '/research/' | relative_url }}">Explore my research <span aria-hidden="true">→</span></a></p>

## News

<ul class="news-list">
  <li><time datetime="2026-09">Sep 2026</time><span>Our paper on <a href="https://papers.miccai.org/miccai-2026/0462-Paper1067.html">hierarchical memory for radiology report generation</a> was published in the <strong>MICCAI 2026</strong> proceedings.</span></li>
  <li><time datetime="2026-05">May 2026</time><span>We released <a href="https://arxiv.org/abs/2605.15128">MemEye</a>, our evaluation framework for multimodal agent memory, on arXiv.</span></li>
</ul>

## Selected work

<p class="section-caption">Memory architectures, evaluation, and a shared view of the field.</p>
{% for id in site.data.featured %}
  {% assign paper = site.data.publications | where: 'id', id | first %}
  {% include publication-entry.html paper=paper %}
{% endfor %}

<p class="section-more"><a href="{{ '/publications/' | relative_url }}">View all publications <span aria-hidden="true">→</span></a></p>

## Education

{% include education.html %}
