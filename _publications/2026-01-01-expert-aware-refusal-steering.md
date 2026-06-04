---
title: "Expert-Aware Refusal Steering"
collection: publications
category: preprints
permalink: /publication/2026-01-01-expert-aware-refusal-steering
excerpt: 'We extend activation addition (ActAdd) refusal steering to Mixture-of-Experts (MoE) architectures and introduce expert-aware steering methods that leverage refusal-specific routing patterns. We find that refusal behavior is distributed across attention and feed-forward sublayers rather than concentrated in MoE experts, and that expert routing patterns do not predict steering effectiveness. Evidence points to two distinct refusal pathways and behavioral entanglement consistent with superposition in post-trained models.'
date: 2026-01-01
venue: 'Under review, Conference on Language Modeling (COLM 2026)'
paperurl: '/files/MoE_Steering_COLM_preprint.pdf'
citation: 'Marbut, A. C., Wheeler, T. J., &amp; Olson, D. R. (2026). &quot;Expert-Aware Refusal Steering.&quot; <i>Preprint under review.</i>'
---

Safety alignment in instruction-tuned LLMs depends on reliable refusal behavior. Recent work has shown that a steering vector applied during inference can suppress refusal in dense models. We extend this method to three open-source Mixture-of-Experts (MoE) LLMs and investigate how the complex routing patterns of MoE architectures interact with steering.

**Key findings:**

- Steering performance is uninhibited by MoE routing patterns — dense-model methods transfer directly
- Refusal behavior is distributed across **both attention and feed-forward sublayers**, not concentrated in specialized experts
- Expert routing patterns don't predict which directions are effective for steering (detection ≠ response)
- We find evidence of **two distinct refusal pathways**: an FFN-mediated pathway (internal) and an attention-mediated pathway (contextual)
- Evidence of **behavioral entanglement** — interference between refusal and adjacent behavioral dimensions — consistent with superposition in post-trained models

We propose two expert-aware steering methods leveraging refusal-specific routing patterns and expert-specific steering directions. The disconnect between where refusal "lives" in routing space and where it can be effectively steered has implications for understanding how alignment generalizes across architectures.
