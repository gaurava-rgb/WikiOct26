---
type: concept
title: Answer Inference vs Agentic Inference
status: developing
created: 2026-09-29
updated: 2026-09-29
tags:
  - concept
source_count: 7
card: true
---

# Answer Inference vs Agentic Inference

**In one sentence:** Thompson splits inference (running a trained AI model) into answer inference, which gives a waiting person an answer, and agentic inference, which does a task. ([[2026-05-11-The-Inference-Shift|The Inference Shift]])

## Why it matters
Thompson argues speed matters most for answers, but memory matters most for agents, because agents must hold their context, state, and history. ([[2026-05-11-The-Inference-Shift|The Inference Shift]]) He predicts agentic inference will be the largest market by far, because it is not limited by people or by time. ([[2026-05-11-The-Inference-Shift|The Inference Shift]]) So he expects it to favor cheap, large memory and good-enough chips, where fast CPUs (general-purpose chips) for tool use matter more than fast GPUs (AI chips). ([[2026-05-11-The-Inference-Shift|The Inference Shift]])

## Worked example: Intel, April 2026
Intel's Lip-Bu Tan said data centers used to pair 1 CPU with every 8 GPUs, now pair 1 with every 4, and are heading toward one for one. ([[2026-04-29-Intel-Earnings-Intels-Differentiation-Whither-Terafab|Intel earnings]]) Thompson says this makes sense: training is bound by GPUs, but inference means many short jobs to coordinate, and agents add tool use on top. ([[2026-04-29-Intel-Earnings-Intels-Differentiation-Whither-Terafab|Intel earnings]]) The same pull showed up at Apple, where agent tools that lean on the CPU caused Mac Mini and Mac Studio shortages. ([[2026-05-06-Microsoft-Earnings-Apple-Earnings|Microsoft and Apple earnings]]) Even Nvidia now ships separate memory and CPU racks for agent work. ([[2026-05-11-The-Inference-Shift|The Inference Shift]])

## Where analysts disagree
- Nvidia's Colette Kress said in May 2026 that mainstream AI has already moved to agentic. ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia earnings, May]]) Thompson says today's agents are still fancy answer inference with a person in the loop. ([[2026-05-11-The-Inference-Shift|The Inference Shift]])
- Jensen Huang said agentic AI has made demand go parabolic (shoot almost straight up). ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia earnings, May]]) Thompson argues Nvidia's edge is speed, so if speed stops being the limit, its chips seem less worth a premium price. ([[2026-05-11-The-Inference-Shift|The Inference Shift]])

## Used in
- [[stories/ai-shift-2024-2026|The AI shift, 2024 to 2026]]: explains which chip makers win next.
- [[journeys/apple-journey|Apple journey]]: agent work sold out Macs.
- [[journeys/amazon-journey|Amazon journey]]: inference shift eases AWS training worries.

## Sources
[[2026-04-20-TSMC-Earnings-New-N3-Fabs-The-Nvidia-Ramp|TSMC earnings]] · [[2026-04-29-Intel-Earnings-Intels-Differentiation-Whither-Terafab|Intel earnings]] · [[2026-05-06-Microsoft-Earnings-Apple-Earnings|Microsoft and Apple earnings]] · [[2026-05-11-The-Inference-Shift|The Inference Shift]] · [[2026-05-14-Interview-Ben-Thompson-MoffettNathanson|MoffettNathanson interview]] · [[2026-05-27-The-SpaceX-IPO-and-Data-Centers-in-Space|The SpaceX IPO]] · [[2026-07-14-The-OpenAI-Super-App-ChatGPT-Codex-Whither-Chat|The OpenAI Super App]]

## Change log
- 2026-09-29: first build from proposal 2026-09-29.

<!-- claims: clm-e7b3dba4d8c3a8965bd2, clm-3d24ff2bf45f6bc73d68, clm-05cf088c008cfb451b3e, clm-ff02535ae1e20260cd69, clm-e5b61f4133ce0abbaceb, clm-d82b30c00bc530806b9a, clm-3c00a13f2af91394f6d6, clm-7fd1c661cf9d29d13017, clm-1b40279b3d0597b3cde4, clm-b213042c1a5b496169c1, clm-e1ca90a02f8e1fcca1c6, clm-77ef3ae7f896d93b3984 -->
