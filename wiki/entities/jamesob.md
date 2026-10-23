---
type: entity
title: jamesob
status: developing
created: 2026-09-29
updated: 2026-10-23
tags:
  - entity
  - entity/person
claim_count: 23
---

# jamesob

Software developer who publishes the local-llm GitHub guide on running state-of-the-art AI models on home hardware.

## Facts by source

### 2026-07-05 [[2026-07-05-jamesob-local-llm-Running-LLMs-Locally|jamesob/local-llm: Everything I know about running LLMs locally]]

- jamesob pitches local AI as an answer to dependence on the big labs, saying that if Dario Amodei and Sam Altman give you heartburn, they should. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-e846a64f99d35b12dff1|cite]])
- jamesob says about $2k buys two RTX 3090 GPUs with 48GB of GPU memory in total, enough to run the Qwen3.6-27B model, which he calls awesome. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-6c52609d4f94c6922a5c|cite]])
- jamesob says about $40k buys the next step up in model intelligence, something he rates as pretty close to Claude Opus. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-878821e35fa30cedf803|cite]])
- At the $40k level, jamesob's pick is four RTX PRO 6000 GPUs for 384GB of GPU memory in total. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-18f0f7cca2bb19b008f8|cite]])
- jamesob names a compressed 594-billion-parameter GLM-5.2 model as the best model for four RTX PRO 6000s as of July 2026, served at about 80 tokens per second with a 460k-token context window. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-e870c97e7d499849a009|cite]])
- jamesob's four RTX PRO 6000 Blackwell GPUs (96GB each) cost about $46,000, which is where most of the money went. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-a0d79b5725dabcd2b634|cite]])
- jamesob says he bought his four RTX PRO 6000s back when they were cheaper. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-ff33ef18704ecc3b3995|cite]])
- Because computer memory had become so expensive, jamesob built a last-generation DDR4 system from eBay parts to host the GPUs and keep the base system cheap. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-e9938f1176fe8490822d|cite]])
- jamesob says a new PCIe5 and DDR5 base system was terrifically expensive as of July 2026, so he spent on GPU memory, where it counts, instead. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-adfc9d79876f6b3c38dd|cite]])
- jamesob's base system, a last-generation AMD EPYC Milan server with 128GB of DDR4 memory, cost $5,587 in parts, mostly from eBay. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-02a6b96d2b1d8d435189|cite]])
- jamesob used PCIe Gen4 switches from indie maker c-payne so the GPUs can exchange data directly at wire speed, cutting latency without costly PCIe5 hardware. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-8fe7547a5cf7ed4c4f62|cite]])
- The c-payne PCIe switch parts cost about 1,220 euros, roughly $1,330. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-a26c6edcfb84160a25d5|cite]])
- With the switch working, jamesob measured GPU-to-GPU transfers of 27.5 GB/s one way and 50.4 GB/s both ways with under a microsecond of latency, the full Gen4 line rate. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-9d616957e40272661d68|cite]])
- jamesob warns that with the default ACS setting on, GPU traffic gets bounced through the CPU instead of staying in the switch, negating the switch entirely. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-bb5068a7600e9fbcc484|cite]])
- jamesob says that without turning IOMMU off, NVIDIA's NCCL multi-GPU library hangs when GPUs talk directly to each other. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-ea07086053c4e1d272d8|cite]])
- To avoid installing a 220V circuit, jamesob runs the rig on a single 110V household circuit and caps each GPU at 350W instead of the default 600W. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-a8dac041c66ea82fe70a|cite]])
- jamesob admits running the rig on a single 110V circuit is probably unwise. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-b69c13af71e86d317b39|cite]])
- A cheap-cable mistake cost jamesob time: an Amazon SAS cable that looked the same as c-payne's differed slightly and caused problems until he reordered. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-a1ce636f76fd4625e79a|cite]])
- jamesob stores all model weights on a mirrored ZFS filesystem across two 8TB drives, downloads them from Hugging Face, and runs each model in its own Docker container. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-db789676df03e09214a4|cite]])
- jamesob argues a key to making open source models good is tooling them properly, giving his agent web search, a Telegram bot for alerts, and a private Gitea code server. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-13b9be0c56d326325251|cite]])
- jamesob's coding agent runs opencode in a sandboxed VM that talks to the host only through a shared folder, so it can install whatever it wants, and it can work Gitea issues and file pull requests on its own. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-8282281b9e829b464509|cite]])
- jamesob finds local speech-to-text with whisper-large-v3 surprisingly useful and says he feels comfortable using it, unlike a hosted equivalent; it needs only about 11GB of GPU memory. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-5813fb78ba7f869dd5e1|cite]])
- jamesob suggests an alternative: a linked cluster of four DGX Spark machines with 512GB of memory as a slow, big brain driving a small Qwen model for quick rote tasks. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-cd318b4424d21569c346|cite]])

## Related concepts

[[AI-Agents|AI Agents]], [[AI-Compute-Demand|AI Compute Demand vs Supply]], [[Local-Inference|Local Inference (Running AI Models on Your Own Hardware)]]
