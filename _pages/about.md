---
permalink: /
title: "Anna Marbut"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a computational linguist and AI researcher studying the geometry and mechanisms of transformer language models. I recently completed my PhD at the University of Montana, where my dissertation — *Searching for Nooks and Crannies: Geometric and Mechanistic Perspectives on Transformer Language Model Interpretability* — examined what the spatial structure of learned representations reveals about model behavior.

I'm currently a Professor of Practice in Applied AI at the University of San Diego.

## Research

My work is organized around a central question: what does the geometry of what language models learn tell us about how and why they behave the way they do?

**Representation geometry.** I've developed and evaluated measures of data spread in high-dimensional embedding spaces, finding that widely-used isotropy measures (ACS, I(V)) are unreliable estimators. I introduced EEE (Eigenvalue Early Enrichment) and VRM (Vasicek Ratio MSE) as more reliable alternatives ([ICML 2023](/publication/2023-07-01-reliable-measures-spread)). I've also found that quantized cell density — which I call Point Patchiness — predicts GLUE benchmark performance with r = 0.9 across BERT-family models ([arXiv:2406.12159](/publication/2024-06-01-latent-space-geometry)).

**Alignment and steering.** I extended ActAdd refusal steering to three open-source Mixture-of-Experts (MoE) architectures and proposed expert-aware steering methods that leverage refusal-specific routing patterns. Key findings: refusal behavior is distributed across both attention and feed-forward sublayers — not concentrated in MoE experts — and expert routing patterns don't reliably predict steering effectiveness. I also found evidence of two distinct refusal pathways (FFN-mediated and attention-mediated) and behavioral entanglement consistent with superposition in post-trained models ([under review, COLM 2026](/publication/2026-01-01-expert-aware-refusal-steering)).

**Weight distributions.** I explored how pre-training scale, task, and hyperparameters shape weight distributions across a range of transformer models, finding that scale and hyperparameter choices affect distributions more than training task. This connects to the lottery ticket hypothesis and has implications for understanding which parts of a network are doing meaningful work.

## Dissertation

*Searching for Nooks and Crannies: Geometric and Mechanistic Perspectives on Transformer Language Model Interpretability* (University of Montana, 2026)

The title comes from a guiding intuition: that the features and behaviors encoded in transformer models are distributed across the high-dimensional spaces they inhabit in a structured, non-uniform way — organized into clusters within clusters, like the memory palace of a building you know well. The dissertation develops this intuition from two directions: geometric analysis of representation spaces in encoder models, and mechanistic analysis of refusal and alignment behavior in decoder MoE models.
