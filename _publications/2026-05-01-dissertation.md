---
title: "Searching for Nooks and Crannies: Geometric and Mechanistic Perspectives on Transformer Language Model Interpretability"
collection: publications
category: dissertations
permalink: /publication/2026-05-01-dissertation
excerpt: 'PhD dissertation (University of Montana, 2026). Examines transformer language model interpretability from two complementary perspectives: geometric analysis of representation spaces in encoder-only models, and mechanistic analysis of refusal and alignment behavior in decoder MoE models.'
date: 2026-05-01
venue: 'University of Montana'
citation: 'Marbut, A. C. (2026). &quot;Searching for Nooks and Crannies: Geometric and Mechanistic Perspectives on Transformer Language Model Interpretability.&quot; PhD dissertation, University of Montana.'
---

**PhD Dissertation, University of Montana (Computational Linguistics, Interdisciplinary), 2026**

The title reflects a central intuition: features and behaviors encoded in transformer models are distributed across high-dimensional spaces in a structured, non-uniform way — organized into clusters within clusters, analogous to a memory palace. The dissertation develops this intuition from two directions.

**Part I — Internal Representations and Weight Distributions (encoder-only models)**

*Chapter 2* proposes and evaluates alternative measures of data spread in high-dimensional latent spaces, introducing EEE and VRM as more reliable alternatives to existing isotropy measures (published at ICML 2023).

*Chapter 3* applies geometric measures to BERT-family model latent spaces and finds that quantized cell density (Point Patchiness) predicts GLUE performance with r = 0.9 (arXiv:2406.12159).

*Chapter 4* explores weight distributions across different pre-training scales, tasks, and hyperparameters, finding that scale and hyperparameter choices affect distributions more than training task does — with connections to the lottery ticket hypothesis.

**Part II — Alignment and Refusal Behavior (decoder MoE models)**

*Chapter 6* extends ActAdd refusal steering to MoE architectures and introduces expert-aware steering methods. It finds evidence of two distinct refusal pathways, behavioral entanglement, and a disconnect between where refusal is detectable and where it can be steered (submitted to COLM 2026).

**Discussion**

The dissertation closes with a speculative theory of recursive clustered structure in latent space ("nooks and crannies"), connecting the geometric findings from Part I to the behavioral findings from Part II. It proposes the linear representation hypothesis extends from semantic content to behavioral dispositions, and that post-training feature entanglement may reflect limited representational capacity at current training scales.
