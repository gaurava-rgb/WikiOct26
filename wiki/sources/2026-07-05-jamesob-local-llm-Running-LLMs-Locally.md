---
type: source
title: "jamesob/local-llm: Everything I know about running LLMs locally"
status: evergreen
created: 2026-09-29
updated: 2026-09-29
tags:
  - source
  - source/article
author: jamesob
published: 2026-07-05
publisher: GitHub
url: "https://github.com/jamesob/local-llm"
raw: .raw/captured/jamesob_local-llm_ Everything I know about running LLMs locally.md
source_id: src-9e7a03fe6483eabcc079
---

# jamesob/local-llm: Everything I know about running LLMs locally

jamesob, GitHub, published 2026-07-05.

## Summary

A hands-on GitHub guide by developer jamesob on running state-of-the-art AI models at home instead of relying on Anthropic or OpenAI. He sets two budgets: about $2k (two used RTX 3090s, 48GB of GPU memory) runs Qwen3.6-27B and local speech-to-text, while about $40k (four RTX PRO 6000s, 384GB) runs a compressed GLM-5.2 model he calls close to Claude Opus. Because memory prices were high in July 2026, he spent on GPU memory and built the rest from cheap last-generation eBay parts, using an indie PCIe switch so the GPUs talk directly to each other. The guide details the fiddly BIOS, kernel and power settings, and argues open models become useful only when given good tools inside a sandboxed agent setup.

## Key claims

- jamesob pitches local AI as an answer to dependence on the big labs, saying that if Dario Amodei and Sam Altman give you heartburn, they should. (§ jamesob's guide to running SOTA LLMs locally: “If Dario and Altman are giving you heartburn (they should be)”) ^clm-e846a64f99d35b12dff1
- jamesob says about $2k buys two RTX 3090 GPUs with 48GB of GPU memory in total, enough to run the Qwen3.6-27B model, which he calls awesome. (§ ~$2k: “2x RTX 3090s for a total of 48GB VRAM total”) ^clm-6c52609d4f94c6922a5c
- jamesob says about $40k buys the next step up in model intelligence, something he rates as pretty close to Claude Opus. (§ ~$40k: “you get the next step up in model intelligence. Something pretty close to Claude Opus”) ^clm-878821e35fa30cedf803
- At the $40k level, jamesob's pick is four RTX PRO 6000 GPUs for 384GB of GPU memory in total. (§ ~$40k: “You'd buy 4x RTX 6000 Pros for a total of 384GB of VRAM”) ^clm-18f0f7cca2bb19b008f8
- jamesob names a compressed 594-billion-parameter GLM-5.2 model as the best model for four RTX PRO 6000s as of July 2026, served at about 80 tokens per second with a 460k-token context window. (§ Contents: “vLLM docker-compose, DCP4+MTP5, ~80 t/s @ 460k ctx”) ^clm-e870c97e7d499849a009
- jamesob's four RTX PRO 6000 Blackwell GPUs (96GB each) cost about $46,000, which is where most of the money went. (§ Contents: “4× RTX PRO 6000, 384GB VRAM (where the money went)”) ^clm-a0d79b5725dabcd2b634
- jamesob says he bought his four RTX PRO 6000s back when they were cheaper. (§ My setup: “I was lucky/dumb enough to buy 4x RTX Pro 6000s back when they were cheaper”) ^clm-ff33ef18704ecc3b3995
- Because computer memory had become so expensive, jamesob built a last-generation DDR4 system from eBay parts to host the GPUs and keep the base system cheap. (§ My setup: “Because RAM is now so expensive, I opted to build a last-gen DDR4 system”) ^clm-e9938f1176fe8490822d
- jamesob says a new PCIe5 and DDR5 base system was terrifically expensive as of July 2026, so he spent on GPU memory, where it counts, instead. (§ My setup: “rather than on a PCIe5/DDR5 base system, which is terrifically expensive as of July 2026”) ^clm-adfc9d79876f6b3c38dd
- jamesob's base system, a last-generation AMD EPYC Milan server with 128GB of DDR4 memory, cost $5,587 in parts, mostly from eBay. (§ Contents: “Last-gen EPYC + eBay DDR4 for $5.6k”) ^clm-02a6b96d2b1d8d435189
- jamesob used PCIe Gen4 switches from indie maker c-payne so the GPUs can exchange data directly at wire speed, cutting latency without costly PCIe5 hardware. (§ My setup: “reduced latency between the cards with less of a need for expensive PCIe5 hardware”) ^clm-8fe7547a5cf7ed4c4f62
- The c-payne PCIe switch parts cost about 1,220 euros, roughly $1,330. (§ Base system: “c-payne Microchip Switchtec PM40100 Gen4 (see sub-BOM below)”) ^clm-a26c6edcfb84160a25d5
- With the switch working, jamesob measured GPU-to-GPU transfers of 27.5 GB/s one way and 50.4 GB/s both ways with under a microsecond of latency, the full Gen4 line rate. (§ Result: “27.5 GB/s unidirectional / 50.4 GB/s bidirectional, 0.37–0.45 µs latency”) ^clm-9d616957e40272661d68
- jamesob warns that with the default ACS setting on, GPU traffic gets bounced through the CPU instead of staying in the switch, negating the switch entirely. (§ ACS Disable (critical for switch P2P): “P2P traffic gets bounced through the CPU root port instead of staying inside the switch fabric”) ^clm-bb5068a7600e9fbcc484
- jamesob says that without turning IOMMU off, NVIDIA's NCCL multi-GPU library hangs when GPUs talk directly to each other. (§ nvidiauvm P2P fix: “Without iommu=off, NCCL hangs on multi-GPU P2P”) ^clm-ea07086053c4e1d272d8
- To avoid installing a 220V circuit, jamesob runs the rig on a single 110V household circuit and caps each GPU at 350W instead of the default 600W. (§ GPU Power Limiting: “350W per GPU (default 600W)”) ^clm-a8dac041c66ea82fe70a
- jamesob admits running the rig on a single 110V circuit is probably unwise. (§ GPU Power Limiting: “I (probably unwisely) run this rig on a single 110V circuit”) ^clm-b69c13af71e86d317b39
- A cheap-cable mistake cost jamesob time: an Amazon SAS cable that looked the same as c-payne's differed slightly and caused problems until he reordered. (§ Picking the right SAS cables: “There was actually a slight difference that was causing issues”) ^clm-a1ce636f76fd4625e79a
- jamesob stores all model weights on a mirrored ZFS filesystem across two 8TB drives, downloads them from Hugging Face, and runs each model in its own Docker container. (§ Hoarding model weights: “I save all model weights locally on a ZFS filesystem”) ^clm-db789676df03e09214a4
- jamesob argues a key to making open source models good is tooling them properly, giving his agent web search, a Telegram bot for alerts, and a private Gitea code server. (§ The harness itself: “One key to making the opensource models good is tooling them properly”) ^clm-13b9be0c56d326325251
- jamesob's coding agent runs opencode in a sandboxed VM that talks to the host only through a shared folder, so it can install whatever it wants, and it can work Gitea issues and file pull requests on its own. (§ The harness itself: “the only communication back to the host system happens via a shared filesystem mount”) ^clm-8282281b9e829b464509
- jamesob finds local speech-to-text with whisper-large-v3 surprisingly useful and says he feels comfortable using it, unlike a hosted equivalent; it needs only about 11GB of GPU memory. (§ ~$2k: “I feel comfortable using it, unlike a hosted equivalent”) ^clm-5813fb78ba7f869dd5e1
- jamesob suggests an alternative: a linked cluster of four DGX Spark machines with 512GB of memory as a slow, big brain driving a small Qwen model for quick rote tasks. (§ Other approaches: “use that as the slow, big brain to drive Qwen3.7-27b to do the rote tasks quickly”) ^clm-cd318b4424d21569c346

## Entities

[[AMD|AMD]], [[Anthropic|Anthropic]], [[Dario-Amodei|Dario Amodei]], GLM, [[Hugging-Face|Hugging Face]], [[Nvidia|Nvidia]], [[OpenAI|OpenAI]], [[Qwen|Qwen]], [[Sam-Altman|Sam Altman]], [[c-payne|c-payne]], [[jamesob|jamesob]]

## Concepts

[[AI-Agents|AI Agents]], [[AI-Compute-Demand|AI Compute Demand vs Supply]], Local Inference (Running AI Models on Your Own Hardware)
