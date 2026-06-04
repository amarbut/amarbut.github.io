---
title: "Reliable Measures of Spread in High Dimensional Latent Spaces"
collection: publications
category: conferences
permalink: /publication/2023-07-01-reliable-measures-spread
excerpt: 'We evaluate existing isotropy measures for high-dimensional text embedding spaces and find that widely-used measures (ACS, I(V)) are unreliable estimators of data spread. We introduce two alternatives — Eigenvalue Early Enrichment (EEE) and Vasicek Ratio MSE (VRM) — that better capture the geometric structure of learned representations.'
date: 2023-07-23
venue: 'Proceedings of the 40th International Conference on Machine Learning (ICML 2023)'
paperurl: '/files/ICML_Reliable_Measures_of_Data_Spread.pdf'
citation: 'Marbut, A. C., McKinney-Bock, K., &amp; Wheeler, T. J. (2023). &quot;Reliable Measures of Spread in High Dimensional Latent Spaces.&quot; <i>Proceedings of the 40th International Conference on Machine Learning (ICML)</i>.'
---

Measuring the spread of data in high-dimensional latent spaces is essential for understanding the geometric structure of text representations, yet existing isotropy measures have not been rigorously evaluated as estimators. We identify failure modes in two widely-used measures — Average Cosine Similarity (ACS) and the partition function-based I(V) — and show that they are unreliable estimators of actual data spread.

We introduce two alternatives: **Eigenvalue Early Enrichment (EEE)**, which captures the concentration of variance in leading principal components, and **Vasicek Ratio MSE (VRM)**, a nonparametric measure derived from order statistics. Both provide more reliable signal about the geometric structure of embedding spaces.

This work is foundational to the broader project of using geometric properties of latent spaces to understand and predict model behavior.
