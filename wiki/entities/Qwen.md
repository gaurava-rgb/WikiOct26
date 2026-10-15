---
type: entity
title: Qwen
status: developing
created: 2026-09-29
updated: 2026-10-15
tags:
  - entity
  - entity/product
claim_count: 8
---

# Qwen

Family of open weight AI models from Alibaba that can run on consumer GPUs.

## Facts by source

### 2026-07-05 [[2026-07-05-jamesob-local-llm-Running-LLMs-Locally|jamesob/local-llm: Everything I know about running LLMs locally]]

- jamesob says about $2k buys two RTX 3090 GPUs with 48GB of GPU memory in total, enough to run the Qwen3.6-27B model, which he calls awesome. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-6c52609d4f94c6922a5c|cite]])
- jamesob suggests an alternative: a linked cluster of four DGX Spark machines with 512GB of memory as a slow, big brain driving a small Qwen model for quick rote tasks. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-cd318b4424d21569c346|cite]])

### 2026-07-20 [[2026-07-20-Whos-Afraid-of-Chinese-Models|Who’s Afraid of Chinese Models?]]

- Per Bloomberg, Alibaba shares rose as much as 5.4% on July 20, 2026 after it released a preview of Qwen3.8 Max, a 2.4 trillion parameter model it called second only to Anthropic's Fable 5; Kimi K3 has 2.8 trillion parameters. ([[2026-07-20-Whos-Afraid-of-Chinese-Models#^clm-bd514ba916acea8b6e28|cite]])
- Alibaba stopped releasing weights for its leading Qwen models earlier in 2026 but reversed course with Qwen3.8 Max, which it plans to make open weight; Thompson ties the shift to a Xi Jinping speech backing open source AI. ([[2026-07-20-Whos-Afraid-of-Chinese-Models#^clm-9adb10286b8bf58b63d6|cite]])

### 2026-10-10 [[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes|GPUs in the Wine Cellar: Why Techies Are Hoarding AI Compute in Their Homes]]

- The YouTuber Digital Spaceport runs a garage home data center with five AMD GPUs, running Alibaba's open model Qwen 3.8 27B to edit and analyze his videos. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-dc478aa8b6b3f0f993f3|cite]])

### 2026-10-12 [[2026-10-12-Researchers-Need-to-Learn-How-AI-Makes-Decisions-Says-Goodfires-Tom-McGrath|Researchers Need to Learn How AI Makes Decisions, Says Goodfire’s Tom McGrath]]

- Goodfire found that open frontier models it studied, including Kimi K3, a big Qwen and a big GLM, hold a fairly coherent internal representation of cheating on a test, which it turned into a very cheap-to-run monitor. ([[2026-10-12-Researchers-Need-to-Learn-How-AI-Makes-Decisions-Says-Goodfires-Tom-McGrath#^clm-06452971368cd694cde3|cite]])
- Goodfire announced an effort to fully reverse-engineer a language model, targeting Alibaba's Qwen3.6-35B-A3B, which is a couple of orders of magnitude smaller than frontier models so experiments cost about 100 times less. ([[2026-10-12-Researchers-Need-to-Learn-How-AI-Makes-Decisions-Says-Goodfires-Tom-McGrath#^clm-3433e08de750d8075436|cite]])
- Prediction: McGrath predicts Goodfire will achieve satisfactory reverse engineering of Qwen3.6-35B-A3B within a year, though not of a frontier-scale model, and expects the method to scale afterward. ([[2026-10-12-Researchers-Need-to-Learn-How-AI-Makes-Decisions-Says-Goodfires-Tom-McGrath#^clm-6d89d216ef1fd4101dca|cite]])

## Related concepts

[[Local-Inference|Local Inference (Running AI Models on Your Own Hardware)]], Mechanistic Interpretability, [[Open-Weight-Models|Open-Weight Models]], [[Reward-Hacking|Reward Hacking]]
