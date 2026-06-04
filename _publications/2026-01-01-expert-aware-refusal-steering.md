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

Safety alignment in instruction-tuned large language models (LLMs) depends on a model's ability to reliably refuse to respond to harmful or disallowed requests. Recent work has shown that a steering vector can be applied to a dense LLM during inference to effectively suppress refusal behavior, inducing response to harmful requests. We extend this refusal steering method to three open-source Mixture-of-Experts (MoE) LLMs and find that steering performance is uninhibited by the complex routing patterns inherent to the MoE architecture. We then propose two expert-aware refusal steering methods that leverage refusal-specific expert routing patterns and expert-specific steering directions to suppress normal refusal behavior. We find that refusal behavior can be effectively steered based on the output of a single expert. Our results show that refusal signals captured by steering methods differ from expert routing behavior, suggesting a substantial role for attention in MoE refusal behavior.
