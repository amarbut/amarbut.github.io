---
title: "Exploring the Impact of a Transformer's Latent Space Geometry on Downstream Task Performance"
collection: publications
category: preprints
permalink: /publication/2024-06-01-latent-space-geometry
excerpt: 'We apply geometric measures to the latent spaces of BERT-family models and find that quantized cell density — Point Patchiness (PP) — has a strong linear relationship (r = 0.9) with GLUE benchmark performance. This suggests that the fine-grained spatial structure of contextual representations is a meaningful predictor of downstream task capability.'
date: 2024-06-18
venue: 'arXiv preprint arXiv:2406.12159'
paperurl: 'https://arxiv.org/abs/2406.12159'
citation: 'Marbut, A. C., Chandler, J., &amp; Wheeler, T. J. (2024). &quot;Exploring the Impact of a Transformer&apos;s Latent Space Geometry on Downstream Task Performance.&quot; <i>arXiv preprint arXiv:2406.12159</i>.'
---

How does the spatial structure of a model's latent representations relate to what it can do? We apply a suite of geometric measures to the contextual embedding spaces of BERT-family models at multiple layers and find a striking result: **quantized cell density**, which we term Point Patchiness (PP), predicts GLUE benchmark performance with r = 0.9.

Point Patchiness captures the degree to which representations cluster into dense local regions within a quantized space — a kind of fine-grained patchwork structure that appears to be diagnostic of representational quality. We also explore non-standard model architectures from the literature and situate these findings within a broader theory of recursive clustered structure in latent space.

This work is a direct predecessor to the "nooks and crannies" framing of latent space geometry developed in my dissertation.

[arXiv:2406.12159](https://arxiv.org/abs/2406.12159)
