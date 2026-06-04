---
permalink: /research/
title: "Research"
author_profile: true
---

My research applies geometric and mechanistic analysis to transformer language models, with the goal of understanding what the structure of learned representations reveals about model behavior and capability.

---

## Representation Geometry in Encoder Models

Transformer language models produce rich contextual representations of the text that they process. These representations are often used directly in downstream tasks and can be used to explore the way that information is extracted and compiled throughout the model. If we think of these representations as individual points in a high-dimensional vector space, we can approach model interpretability from a geometric perspective and use distributional characteristics to better understand how these models function.

To this end, I first focused on quantifying distributional spread: how fully do a model's latent representations use the avilable high-dimensional space? I found that widely-used measures of isotropy (Average Cosine Similarity, I(V)) are unreliable estimators, and introduced EEE (Eigenvalue Early Enrichment) and VRM (Vasicek Ratio MSE) as better alternatives. This matters because spread measures are used to evaluate and compare representation quality, and unreliable measures lead to unreliable conclusions.

Next, I explored measures that would quantify the degree and distribution of clustering within a model's latent representations, and asked the question of whether any of these measures are directly related to downstream model performance. I found that quantized point patchiness, a measure of variability in cluster distributions borrowed from ecology, predicts GLUE performance with r = 0.9 across a series of perturbed BERT-family models. This suggests the fine-grained patchwork structure of contextual representations may be predictively related to downstream model performance.

**Relevant repos:** [`isotropy`](https://github.com/amarbut/isotropy) · [`manifolds`](https://github.com/amarbut/manifolds)

---

## Weight Initialization, Pre-Training, and Model Overparameterization

Most of today's transformer language models follow a two-stage training procedure, first on a general language modeling task (pre-training), and then on a specific downstream task (post-training). This training regime is referred to as "transfer learning", in which the model learns foundational knowledge and skills that set it up for more efficient and effective task-specific training. However, the internal mechanisms that make transfer learning so successful are still poorly understood: is there an identifiable characteristic of the distribution of model weights after pre-training that is beneficial for learning post-training tasks? If so, can we initialize our models with this characteristic in mind to make model pre-training more efficient or to better understand what the model truly learns during pre-training?

In this brief analysis, I explored how pre-training scale, task, and hyperparameters shape the distribution of weights across transformer layers, finding that scale and hyperparameter choices have larger effects than training task. I also performed preliminary experiments and exploratory analyses around the ideas of weight movement and its relation to model overparameterization, exploring the question of whether we can use distributional characteristics of pre-trained model weights to predict weight movement and influence early in pre-training.

**Relevant repo:** [`initialization`](https://github.com/amarbut/initialization)

---

## Refusal Steering in Mixture-of-Experts Models

Safety alignment in generative transformer language models requires that they will reliably refuse to respond to harmful user requests. My most recent project investigates what happens to this behavior in Mixture-of-Experts (MoE) architectures, which are increasingly common at frontier scale.

I extended ActAdd refusal steering to three open-source MoE models and introduced expert-aware steering methods. While expert-aware steering was not as effective as steering based on the aggregated residual stream, my results provided several insights into refusal behavior in MoE models:

- Refusal behavior is distributed across attention and feed-forward sublayers, not localized in experts
- Refusal-specific expert routing patterns don't predict steering effectiveness, suggesting that the refusal signal coming from the MoE routing mechanism is distinct from that used to steer the model's behavior
- There appear to be two distinct refusal pathways: FFN-mediated (learned during alignment post-training) and attention-mediated (incorporated from the model input through a system prompt or otherwise)
- Nonmonotonic steering performance when scaling the intervention suggests behavioral feature entanglement consistent with superposition in post-trained models

**Relevant repo:** [`alignment`](https://github.com/amarbut/alignment)
