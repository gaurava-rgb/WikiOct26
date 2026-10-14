---
type: concept
title: Local Inference (Running AI Models on Your Own Hardware)
status: developing
created: 2026-09-29
updated: 2026-10-13
tags:
  - concept
source_count: 7
card: true
---

# Local Inference (Running AI Models on Your Own Hardware)

**In one sentence:** Running AI on computers you own instead of renting a big lab's model in the cloud, for cost, privacy and convenience. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes|GPUs in the Wine Cellar]])

## Why it matters
It flips AI from a monthly bill to something you buy once. Former Microsoft executive Gary Flake put it simply: "I want to own. I don't want to rent." ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes|GPUs in the Wine Cellar]]) Big firms do it to keep secrets: Nvidia runs sensitive work on its own Nemotron models. ([[2026-09-14-Anthropic-Data-Fears-Prompt-Nvidia-Palantir-and-Booz-Allen-to-Restrict-Model-Use|Anthropic Data Fears]]) It moves hardware: AI labs bought tens of thousands of Mac minis and Mac Studios, causing an extreme shortage. ([[2026-09-16-Apple-Considers-Return-to-Server-Market-Has-Talked-With-Nvidia-to-Use-Network-Tech|Apple Servers]]) The catch: Thompson argues a phone, however powerful, is less capable than the cloud. ([[2026-09-10-The-iPhone-Duo-The-Intelligent-Personal-Hub-Apple-Watch-Audio-Intelligence|iPhone Duo]])

## Worked example: jamesob's home rig, July 2026
About $2,000 buys two RTX 3090 gaming GPUs with 48GB of GPU memory (the fast memory that sets how big a model fits), enough for a good Qwen model. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally|Running LLMs Locally]]) jamesob went bigger: four RTX PRO 6000 GPUs for about $46,000. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally|Running LLMs Locally]]) He hosts them on a last-generation server built from $5,587 of parts, mostly from eBay. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally|Running LLMs Locally]]) He says that tier gets you close to Claude Opus. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally|Running LLMs Locally]])

## Used in
- [[journeys/apple-journey|Apple journey]]: the Mac mini boom and Apple's on-device bet ([[journeys/apple-journey-2025-2026|Apple, 2025 to 2026]])
- See also [[Open-Weight-Models]]: the downloadable models that make it possible

## Sources
[[2026-07-05-jamesob-local-llm-Running-LLMs-Locally|Running LLMs Locally]] · [[2026-09-10-The-iPhone-Duo-The-Intelligent-Personal-Hub-Apple-Watch-Audio-Intelligence|iPhone Duo]] · [[2026-09-14-Anthropic-Data-Fears-Prompt-Nvidia-Palantir-and-Booz-Allen-to-Restrict-Model-Use|Anthropic Data Fears]] · [[2026-09-16-Apple-Considers-Return-to-Server-Market-Has-Talked-With-Nvidia-to-Use-Network-Tech|Apple Servers]] · [[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes|GPUs in the Wine Cellar]]

## Change log
- 2026-10-13: upgraded to an idea card per proposal 2026-10-13.

<!-- claims: clm-c21986d73b9b6f2c73a8, clm-dad52f48b3f6d6153303, clm-3aafd5013488f2437bc6, clm-96f74139d5a6f7903ebb, clm-f96fb0f453a2ef6dcc33, clm-6c52609d4f94c6922a5c, clm-a0d79b5725dabcd2b634, clm-02a6b96d2b1d8d435189, clm-878821e35fa30cedf803 -->
