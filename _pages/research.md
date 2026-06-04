---
permalink: /research/
title: "Research"
author_profile: true
---

My research applies geometric and mechanistic analysis to transformer language models, with the goal of understanding what the structure of learned representations reveals about model behavior and capability.

---

## Representation Geometry in Encoder Models

How is information arranged in the high-dimensional spaces that transformer encoders learn? I've approached this question through two threads.

The first concerns **measuring spread**: how uniform or clustered are the representations in a space? I found that widely-used isotropy measures (Average Cosine Similarity, I(V)) are unreliable estimators, and introduced EEE (Eigenvalue Early Enrichment) and VRM (Vasicek Ratio MSE) as better alternatives. This matters because spread measures are used to evaluate and compare representation quality — unreliable measures lead to unreliable conclusions.

The second concerns **predicting capability from geometry**: can we read off what a model can do from the spatial structure of its representations? We found that quantized cell density — Point Patchiness — predicts GLUE performance with r = 0.9 across BERT-family models. This suggests the fine-grained patchwork structure of contextual representations is diagnostically meaningful.

**Relevant repos:** [`isotropy`](https://github.com/amarbut/isotropy) · [`manifolds`](https://github.com/amarbut/manifolds)

---

## Weight Distributions Across Pre-Training Regimes

Before a model is fine-tuned or evaluated, its weights encode the cumulative effect of pre-training. I explored how pre-training scale, task, and hyperparameters shape the distribution of weights across transformer layers, finding that scale and hyperparameter choices have larger effects than training task.

This analysis connects to the lottery ticket hypothesis — if certain weight patterns reflect the "winning tickets" that survive training, then weight distribution analysis may offer a window into what a model has and hasn't learned to do. It also has practical implications for structured pruning and transfer learning.

**Relevant repo:** [`initialization`](https://github.com/amarbut/initialization)

---

## Refusal Steering in Mixture-of-Experts Models

Safety alignment depends on reliable refusal: a model's ability to decline to respond to harmful or disallowed requests. My most recent project investigates what happens to this behavior in Mixture-of-Experts (MoE) architectures, which are increasingly common at frontier scale.

I extended ActAdd refusal steering to three open-source MoE models and introduced expert-aware steering methods. The findings complicate a simple picture of "refusal experts":

- Refusal behavior is distributed across attention and feed-forward sublayers, not localized in experts
- Expert routing patterns don't predict steering effectiveness — you can detect which experts activate on refusal prompts, but that doesn't tell you how to steer
- There appear to be two distinct refusal pathways: FFN-mediated (responding to the internal content of a request) and attention-mediated (responding to conversational context)
- Interference between refusal and adjacent behavioral dimensions suggests feature entanglement consistent with superposition in post-trained models

**Relevant repo:** [`alignment`](https://github.com/amarbut/alignment)
