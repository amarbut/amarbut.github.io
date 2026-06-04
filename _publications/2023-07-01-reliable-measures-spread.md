---
title: "Reliable Measures of Spread in High Dimensional Latent Spaces"
collection: publications
category: conferences
permalink: /publication/2023-07-01-reliable-measures-spread
excerpt: 'We evaluate existing isotropy measures for high-dimensional text embedding spaces and find that widely-used measures (ACS, I(V)) are unreliable estimators of data spread. We introduce two alternatives, Eigenvalue Early Enrichment (EEE) and Vasicek Ratio MSE (VRM), that better capture the geometric structure of learned representations.'
date: 2023-07-23
venue: 'Proceedings of the 40th International Conference on Machine Learning (ICML 2023)'
paperurl: '/files/ICML_Reliable_Measures_of_Data_Spread.pdf'
citation: 'Marbut, A. C., McKinney-Bock, K., &amp; Wheeler, T. J. (2023). &quot;Reliable Measures of Spread in High Dimensional Latent Spaces.&quot; <i>Proceedings of the 40th International Conference on Machine Learning (ICML)</i>.'
---

Understanding geometric properties of the latent spaces of natural language processing models allows the manipulation of these properties for improved performance on downstream tasks. One such property is the amount of data spread in a model's latent space, or how fully the available latent space is being used. We demonstrate that the commonly used measures of data spread, average cosine similarity and a partition function min/max ratio I(V), do not provide reliable metrics to compare the use of latent space across data distributions. We propose and examine six alternative measures of data spread, all of which improve over these current metrics when applied to seven synthetic data distributions. Of our proposed measures, we recommend one principal component-based measure and one entropy-based measure that provide reliable, relative measures of spread and can be used to compare models of different sizes and dimensionalities.
