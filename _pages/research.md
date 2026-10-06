---
title: Research
permalink: /research/
excerpt: "Research on multimodal memory, agent evaluation, reliable tool use, and memory-augmented generation."
---

I design memory systems, evaluations, and decision-making methods for AI agents. My doctoral research at the **University of Notre Dame**, advised by **[Prof. Yiyu Shi](https://cse.nd.edu/faculty/yiyu-shi/)**, focuses on how agents preserve evidence and use it reliably over time.

<nav class="section-jump" aria-label="Research topics"><a href="#memory">Memory & evaluation</a><a href="#decisions">Agent decisions</a><a href="#generation">Multimodal generation</a></nav>

## Memory & evaluation {#memory}

### MemEye: Evaluating multimodal agent memory

A two-axis benchmark that separates **visual-detail retention** from **reasoning over changing states**, enabling targeted diagnosis of agent memory failures.

- Built a benchmark-construction pipeline with checks for answerability, visual dependence, and textual shortcuts; expanded coverage to **1,200 questions across eight scenarios and 12 categories**.
- Evaluated **13 memory methods across four VLM backbones**, identifying lost visual details, stale retrieval, and state-tracking failures as bottlenecks.

<p class="resource-links"><a href="https://arxiv.org/abs/2605.15128">Paper ↗</a><a href="{{ '/publications/#memeye' | relative_url }}">Publication details →</a></p>

### Seeing, Maintaining, and Learning

A unified taxonomy of how multimodal agents represent experience, adapt memory management, and learn from accumulated experience and feedback, connecting architectural choices with evaluation needs.

- Co-developed a **two-axis taxonomy** connecting memory formation and representation with management adaptivity, distinguishing static, dynamic, and self-evolving memory systems.
- Curated **296 memory architectures and 83 evaluation resources across five modality categories**; analyzed evidence preservation, storage efficiency, and temporal consistency.

<p class="resource-links"><a href="https://openreview.net/forum?id=5u8ag6LBFH">OpenReview ↗</a><a href="https://github.com/Seeing-Maintaining-Learning/multimodal-agent-memory-survey">Survey resources ↗</a></p>

## Reliable agent decisions {#decisions}

### Agent Last Doubt: Risk-aware tool use

A framework for tool-using LLM agents to **clarify, search, act, or escalate under uncertainty**, balancing expected task success, interaction cost, and irreversible error risk.

- Designed an action-conditioned value model that predicts success, cost, and critical errors separately, enabling configurable inference-time trade-offs without retraining the backbone.
- Built a counterfactual rollout pipeline on **ToolSandbox and τ²-bench** to compare alternative interventions from identical snapshots and generate outcome-based supervision.

### Node-as-Agent: Graph Agentic Network

**ReaGAN** is a training-free, LLM-powered Node-as-Agent framework for node classification, combining local graph aggregation with global retrieval.

- Designed local-global memory that combines graph-neighbor evidence with semantically relevant nodes retrieved through RAG.
- Evaluated a frozen **Qwen2.5-14B** model on Cora, Citeseer, and Chameleon; achieved **84.95% accuracy on Cora** without task-specific fine-tuning.

<p class="resource-links"><a href="https://arxiv.org/abs/2508.00429">Paper ↗</a></p>

## Multimodal generation {#generation}

### Hierarchical memory for radiology report generation

**HM-RRG** combines hierarchical memory and retrieval-augmented generation to ground chest X-ray reports in similar cases and longitudinal patient histories.

- Implemented image-conditioned memory compression, segment-level retrieval, and **LoRA-based fine-tuning of BioMistral-7B**.
- Improved CheXbert clinical F1 from **0.483 to 0.580** over flat context concatenation on MIMIC-CXR, a **20.1% relative improvement**.

<p class="resource-links"><a href="https://papers.miccai.org/miccai-2026/0462-Paper1067.html">MICCAI 2026 paper ↗</a><a href="https://github.com/QingyueJ-nd/HM-RRG">Code ↗</a></p>

### MediQ-GAN: Medical image generation from limited data

A prototype-conditioned hybrid GAN combining classical and quantum-inspired modules for **synthetic data augmentation** of underrepresented medical image classes.

- Ran augmentation experiments across three datasets and two classifier backbones; improved ViT-small accuracy on ISIC2019 from **72.49% to 82.60%**.
- Analyzed generator Jacobian spectra and effective rank to diagnose mode collapse and characterize latent-space utilization.

<p class="resource-links"><a href="https://arxiv.org/abs/2506.21015">Paper ↗</a></p>
