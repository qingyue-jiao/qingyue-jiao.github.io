---
title: "About me"
permalink: /
excerpt: "Qingyue Jiao — AI agents, multimodal memory, and reliable decision-making. Open to research and engineering internships."
---

I am a third-year Ph.D. candidate in **Computer Science and Engineering at the University of Notre Dame**, advised by **[Prof. Yiyu Shi](https://cse.nd.edu/faculty/yiyu-shi/)**.

I build and evaluate systems that help **AI agents remember, reason, and make reliable decisions**, with a focus on multimodal memory, retrieval-augmented generation, and decision-making under uncertainty.

<div class="availability">I am open to <strong>research collaborations and internship opportunities</strong>—please feel free to <a href="mailto:qjiao@nd.edu">get in touch</a>.</div>


## Selected work

{% for id in site.data.featured %}
  {% assign paper = site.data.publications | where: 'id', id | first %}
  {% include publication-entry.html paper=paper %}
{% endfor %}

<p class="section-more"><a href="{{ '/research/' | relative_url }}">Research &amp; projects →</a> · <a href="{{ '/publications/' | relative_url }}">All publications →</a></p>

## News

<ul class="news-list">
  <li><time datetime="2026-09">Sep 2026</time><span>Our paper on <a href="https://papers.miccai.org/miccai-2026/0462-Paper1067.html">hierarchical memory for radiology report generation</a> was published in the <strong>MICCAI 2026</strong> proceedings.</span></li>
  <li><time datetime="2026-05">May 2026</time><span>We released <a href="https://arxiv.org/abs/2605.15128">MemEye</a>, our evaluation framework for multimodal agent memory, on arXiv.</span></li>
</ul>
