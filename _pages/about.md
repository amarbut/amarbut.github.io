---
permalink: /
title: "Anna Marbut"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a computational linguist and AI interpretability researcher focused on understanding transformer language model behavior through the geometry of internal model representations. I recently completed my PhD at the University of Montana, where my dissertation, *Searching for Nooks and Crannies: Geometric and Mechanistic Perspectives on Transformer Language Model Interpretability*, examined what the spatial structure of learned representations reveals about model behavior.

I'm currently a Professor of Practice in Applied AI at the University of San Diego.

## Research

My work is organized around a central question: what does the geometry of what language models learn tell us about how and why they behave the way they do?

**Representation geometry.** I've developed and evaluated measures of data spread in high-dimensional embedding spaces, finding that widely-used isotropy measures (ACS, I(V)) are unreliable estimators. I introduced EEE (Eigenvalue Early Enrichment) and VRM (Vasicek Ratio MSE) as more reliable alternatives ([ICML 2023](/publication/2023-07-01-reliable-measures-spread)). I've also found that quantized cell density predicts GLUE benchmark performance with r = 0.9 across a series of synthetically perturbed BERT-family models ([arXiv:2406.12159](/publication/2024-06-01-latent-space-geometry)).

**Alignment and steering.** I extended ActAdd refusal steering to three open-source Mixture-of-Experts (MoE) architectures and proposed expert-aware steering methods that leverage refusal-specific routing patterns. I found that refusal behavior is distributed across both attention and feed-forward sublayers and that expert routing patterns don't reliably predict steering effectiveness. I also found evidence of two distinct refusal pathways (FFN-mediated and attention-mediated) and behavioral entanglement consistent with superposition in post-trained models ([under review, COLM 2026](/publication/2026-01-01-expert-aware-refusal-steering)).

**Weight distributions.** I explored how pre-training scale, task, and hyperparameters shape weight distributions across a range of transformer models, finding that scale and hyperparameter choices affect distributions more than training task. This connects to the lottery ticket hypothesis and has implications for understanding which parts of a network are doing meaningful work.

## Dissertation

*Searching for Nooks and Crannies: Geometric and Mechanistic Perspectives on Transformer Language Model Interpretability* (University of Montana, 2026)

The title comes from a guiding intuition: that the features and behaviors encoded in transformer models are organized within a complex internal structure in the model's high-dimensional latent space that, like the nooks and crannies of a physical space, provides distinct regions that can be used to store and separate information. The dissertation develops this intuition from two directions: geometric analysis of representation spaces in encoder models, and mechanistic analysis of refusal and alignment behavior in decoder MoE models.
