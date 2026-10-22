---
title: "Interpretability Is the Key to Physical AI, Says World Mechanics CEO Sonia Joseph"
author: Rocket Drew
publication: The Information
published: 2026-10-19
url: https://www.theinformation.com/articles/interpretability-key-physical-ai-says-world-mechanics-ceo-sonia-joseph
kind: reading-notes
note: "Paraphrased notes with short quotes, taken from Gaurav's subscription. Not the full article text."
---

# Notes: Interpretability Is the Key to Physical AI, Says World Mechanics CEO Sonia Joseph

The Information, Rocket Drew, 2026-10-19 (interview).

## The connection between world models and mechanistic interpretability

- Sonia Joseph, co-founder and CEO of startup World Mechanics and former head of Meta's interpretability forum, argues that world models and mechanistic interpretability are two sides of the same coin.
- She distinguishes the East Coast definition of world models (rooted in neuroscience and internal representations that map to physical reasoning) from the West Coast definition (focused on video realism or robotics control).
- Joseph argues that effective world models require internal representations that are disentangled, causal, and map directly to physical laws.
- Without white-box interpretability, physical AI models can rely on spurious cues, like a surgeon's mask color or rings on fingers during robotic surgery.

## Interpretability-guided training versus raw scale

- Probing models internally enables interpretability-guided training, which checks whether a model has learned a concept like object permanence and feeds data dynamically, cutting training data needs significantly.
- Joseph argues this approach is compatible with the bitter lesson: while brute-force compute may eventually find physical representations, interpretability and inductive biases speed up development from years to weeks.
- She proposes distilling large unsupervised video models by using reinforcement learning to identify interpretable, causally relevant primitives (such as velocity or mass) and baking them into smaller architectures.
- Joseph cautions that physical AI will not follow language models with one foundation model ruling everything, because continuous physical sensors (temperature, pressure, acoustics) require diverse, specialized intelligences.

## Language limits and physical ground truth

- Unlike language, which has no single mathematical ground truth, the physical world has objective laws like Newtonian dynamics.
- Joseph doubts recursive self-improvement from language models will solve physical AI, calling it a fairy tale because moving physical matter faces real time, slowness, and hardware constraints.
- She discusses Meta's Joint Embedding Predictive Architecture (JEPA), pioneered with Yann LeCun, which predicts abstract representations in latent space rather than raw pixels.
- While respecting LeCun, Joseph differs by insisting on interpretability first, verifying what latent spaces actually represent at each layer.
- Making AI interpretable to blue-collar workers and doctors in high-liability industries (like steel pouring or surgery) is essential for commercial adoption.

## Why it matters for the wiki

- Idea card Mechanistic Interpretability: extends interpretability beyond large language models into robotics, continuous sensor data, and physical validation.
- Idea card World Models: provides a sharp distinction between visual simulation and functional, causally grounded physical reasoning.
- Meta journey: contextualizes Meta's JEPA research and former internal researchers launching specialized startups.
