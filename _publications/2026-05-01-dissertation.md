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

Large language models (LLMs) have demonstrated remarkable linguistic capabilities, but the internal mechanisms driving their performance and behavior remain poorly understood. This dissertation investigates the interpretability of transformer-based language models from two complementary perspectives: the geometric organization of model internals in encoder-only models, and the mechanisms underlying safety behavior in decoder-only generative models.

In Part I, we address the challenge of measuring geometric properties in high-dimensional latent spaces, proposing and evaluating alternative measures of data spread that improve upon commonly used metrics. We then apply these measures alongside quantization-based metrics to examine the relationship between latent space geometry and downstream benchmarking performance, finding that a quantized cell density measure has a strong linear relationship with GLUE performance in a series of synthetically perturbed BERT-family models. We further explore how pre-training data scale, training task, and hyperparameter configuration shape the resulting model weight distributions, observing that training scale and hyperparameter choices have a more pronounced effect on weight distributions than training task.

In Part II, we investigate refusal behavior in Mixture of Experts (MoE) generative models, extending an existing activation steering method to MoE architectures and introducing expert-aware steering methods that isolate the contributions of individual model components. Our results demonstrate that refusal behavior is not localized to the MoE feed-forward sublayer, but is distributed across the feed-forward and attention sublayers, with evidence suggesting two distinct refusal pathways: an internal pathway mediated by the feed-forward sublayer and a contextual pathway mediated by attention. We also observe evidence of post-training behavioral entanglement and non-linear geometry in the model's latent representations.

Together, these findings contribute to a growing understanding of the internal organization of transformer language models and highlight the complexity of the relationship between model internals, downstream performance, and learned behavior.
