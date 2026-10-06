---
title: "Research & Projects"
permalink: /research/
excerpt: "Selected projects, individual contributions, and results in AI agents, multimodal memory, and generation."
---

My research at the **University of Notre Dame**, advised by **[Prof. Yiyu Shi](https://cse.nd.edu/faculty/yiyu-shi/)**, focuses on building and evaluating reliable AI agents. Below are the problems I work on, my contributions, and the resulting systems and findings.

<nav class="section-jump" aria-label="Research topics"><a href="#memory">Memory & evaluation</a><a href="#decisions">Agent decisions</a><a href="#generation">Multimodal generation</a></nav>

## Memory & evaluation {#memory}

### MemEye: Evaluating multimodal agent memory

**Problem.** Agents can lose visual details or retrieve outdated evidence across conversations. Evaluations need to distinguish these failures from reasoning errors.

**My contribution.** Built a **benchmark-construction pipeline** with checks for answerability, visual dependence, and textual shortcuts; expanded coverage to 1,200 questions across eight scenarios and 12 categories.

**Result.** Evaluated **13 memory methods across four VLM backbones**, identifying visual-detail loss, stale retrieval, and state-tracking failures as bottlenecks.

<p class="resource-links"><a href="https://arxiv.org/abs/2605.15128">Paper ↗</a><a href="https://minghokwok.github.io/MemEye/">Project &amp; examples ↗</a><a href="https://github.com/MinghoKwok/MemEye">Code ↗</a><a href="https://huggingface.co/datasets/MemEyeBench/MemEye">Dataset ↗</a></p>

### Seeing, Maintaining, and Learning: Multimodal agent memory survey

**Problem.** Comparing memory systems requires a shared view of how they represent evidence, manage updates, and learn from experience.

**My contribution.** Co-developed a **two-axis taxonomy** connecting memory formation and representation with management adaptivity, distinguishing static, dynamic, and self-evolving systems.

**Result.** Curated **296 memory architectures and 83 evaluation resources across five modality categories**, connecting architectural choices with evidence preservation, storage efficiency, and temporal consistency.

<p class="resource-links"><a href="https://openreview.net/forum?id=5u8ag6LBFH">Paper ↗</a><a href="https://github.com/Seeing-Maintaining-Learning/multimodal-agent-memory-survey">Survey resources ↗</a></p>

## Reliable agent decisions {#decisions}

### Agent Last Doubt: Risk-aware tool use

**Problem.** Tool-using agents must decide when to clarify, search, act, or escalate while balancing task success, interaction cost, and irreversible error risk.

**My contribution.** Designed an **action-conditioned value model** that predicts success, cost, and critical errors separately, supporting configurable inference-time trade-offs with a fixed backbone.

**Output.** Built a **counterfactual rollout pipeline on ToolSandbox and τ²-bench** to compare interventions from identical snapshots and generate outcome-based supervision.

### Node-as-Agent: Graph Agentic Network

**Problem.** Node classification requires combining local graph structure with relevant evidence beyond a node’s immediate neighbors.

**My contribution.** Designed **local-global memory** for ReaGAN, a training-free, LLM-powered Node-as-Agent framework, combining graph-neighbor evidence with semantically relevant nodes retrieved through RAG.

**Result.** Evaluated frozen **Qwen2.5-14B** on Cora, Citeseer, and Chameleon; achieved **84.95% accuracy on Cora** without task-specific fine-tuning.

<p class="resource-links"><a href="https://arxiv.org/abs/2508.00429">Paper ↗</a></p>

## Multimodal generation {#generation}

### HM-RRG: Hierarchical memory for radiology report generation

**Problem.** Generating clinically accurate chest X-ray reports requires selecting relevant evidence from retrieved cases and long patient histories.

**My contribution.** Implemented **image-conditioned memory compression, segment-level retrieval, and LoRA fine-tuning of BioMistral-7B** within a hierarchical memory and RAG framework.

**Result.** Improved CheXbert clinical F1 from **0.483 to 0.580** over flat context concatenation on **MIMIC-CXR**, a 20.1% relative improvement. Published at MICCAI 2026.

<p class="resource-links"><a href="https://papers.miccai.org/miccai-2026/0462-Paper1067.html">Paper ↗</a><a href="https://github.com/QingyueJ-nd/HM-RRG">Code ↗</a></p>

### MediQ-GAN: Medical image generation from limited data

**Problem.** Underrepresented medical image classes can limit classifier performance when training data are scarce.

**My contribution.** Ran **synthetic data augmentation** experiments with a prototype-conditioned hybrid GAN across three datasets and two classifier backbones. Analyzed generator Jacobian spectra and effective rank to diagnose mode collapse and latent-space utilization.

**Result.** Improved **ViT-small accuracy on ISIC2019 from 72.49% to 82.60%** using augmentation with the model’s generated images.

<p class="resource-links"><a href="https://arxiv.org/abs/2506.21015">Paper ↗</a></p>
