---
title: "Exploring the Impact of a Transformer's Latent Space Geometry on Downstream Task Performance"
collection: publications
category: preprints
permalink: /publication/2024-06-01-latent-space-geometry
excerpt: 'We apply geometric measures to the latent spaces of BERT-family models and find that quantized cell density has a strong linear relationship (r = 0.9) with GLUE benchmark performance. This suggests that the fine-grained spatial structure of contextual representations is a meaningful predictor of downstream task capability.'
date: 2024-06-18
venue: 'arXiv preprint arXiv:2406.12159'
paperurl: 'https://arxiv.org/abs/2406.12159'
citation: 'Marbut, A. C., Chandler, J., &amp; Wheeler, T. J. (2024). &quot;Exploring the Impact of a Transformer&apos;s Latent Space Geometry on Downstream Task Performance.&quot; <i>arXiv preprint arXiv:2406.12159</i>.'
---

It is generally thought that transformer-based large language models benefit from pre-training by learning generic linguistic knowledge that can be focused on a specific task during fine-tuning. However, we propose that much of the benefit from pre-training may be captured by geometric characteristics of the latent space representations, divorced from any specific linguistic knowledge. In this work we explore the relationship between GLUE benchmarking task performance and a variety of measures applied to the latent space resulting from BERT-type contextual language models. We find that there is a strong linear relationship between a measure of quantized cell density and average GLUE performance and that these measures may be predictive of otherwise surprising GLUE performance for several non-standard BERT-type models from the literature \cite{alajrami2022does, sinha2021masked, zhang2021general}. These results may be suggestive of a strategy for decreasing pre-training requirements, wherein model initialization can be informed by the geometric characteristics of the model's latent space.

[arXiv:2406.12159](https://arxiv.org/abs/2406.12159)
