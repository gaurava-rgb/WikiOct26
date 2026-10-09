---
type: source
title: The Inference Shift
status: evergreen
created: 2026-09-29
updated: 2026-09-29
tags:
  - source
  - source/article
author: Ben Thompson
published: 2026-05-11
publisher: Stratechery
url: "https://stratechery.com/2026/the-inference-shift/"
raw: .raw/captured/The Inference Shift.md
source_id: src-b73e19487f1c5ee17dd6
---

# The Inference Shift

Ben Thompson, Stratechery, published 2026-05-11.

## Summary

Thompson uses the Cerebras IPO to argue that AI compute is becoming heterogeneous after an era dominated by Nvidia GPUs. He introduces a split between answer inference, where a human waits and speed matters, and agentic inference, where agents work without humans and memory capacity matters more than speed. He predicts agentic inference will be the largest market by far and will unbundle the GPU in favor of big, cheaper memory hierarchies with good-enough compute and fast CPUs. That would weaken Nvidia's latency-driven premium, help China, make space data centers more viable, and make Moore's Law matter less.

## Key claims

- Cerebras was set in May 2026 to raise its IPO price range to $150 to $160 a share, up from $115 to $125, and to market 30 million shares instead of 28 million, as demand for the stock climbed. (“considering a new IPO price range of $150-$160 a share, up from $115-$125 a share”) ^clm-ecadd8a9a01305b7fb0d
- Thompson argues the surge in semiconductor stocks in May 2026 is driven by AI, and especially by the realization that agents will need a lot of compute. (“the realization that agents are going to need a lot of compute”) ^clm-8047fb0392f4f0db1ca5
- Prediction: Thompson argues that while the AI compute story has been mostly about Nvidia GPUs, the future will look increasingly heterogeneous, with different chips for different jobs. (“the future is going to look increasingly heterogeneous”) ^clm-393f3b125092dc1ee893
- Thompson explains that Nvidia leads AI training because it secured high-bandwidth memory (HBM) ahead of rivals and invested in chip-to-chip networking, both needed because every GPU must share results before the next training step. (§ The GPU Era: “first by securing HBM ahead of the rest of the industry”) ^clm-c0420d16b846c9f5b195
- Thompson explains that inference decode is serial and limited by memory bandwidth: for every token generated, both the KV cache (the stored context) and the model weights must be read in full. (§ The GPU Era: “decode is serial and memory-bandwidth bound”) ^clm-a3ff8cc4c714c3f1af74
- Anthropic agreed in May 2026 to use all compute at SpaceX's Colossus 1 data center, over 300 megawatts and more than 220,000 Nvidia GPUs, to raise capacity for Claude Pro and Max subscribers. (§ The GPU Era: “more than 300 megawatts of new capacity (over 220,000 NVIDIA GPUs) within the month”) ^clm-ecf330fefff606b208d4
- Thompson argues SpaceX can run both training and inference at Colossus 2 because xAI's models get little usage and because GPUs can do both jobs; the Colossus 1 GPUs Anthropic rents were first used for training, showing GPU flexibility is a big advantage. (§ The GPU Era: “the fact that GPUs are so flexible is a big advantage”) ^clm-d22c5195160bdd9f365b
- Cerebras lays wiring across the scribe lines between reticle exposures, turning a whole 300mm wafer into one chip with no slow chip-to-chip links, while Nvidia's B200 links two separate chips. (§ Understanding Cerebras: “making the entire wafer into a single chip with no need for relatively slow chip-to-chip linkages”) ^clm-eed97a821606823662fc
- As of May 2026, Cerebras' WSE-3 has 44GB of on-chip SRAM at 21 PB/s of bandwidth, versus 80GB of HBM at 3.35 TB/s on Nvidia's H100: just over half the memory but 6,000 times the bandwidth. (§ Understanding Cerebras: “the WSE-3 has just over half the memory of an H100, but 6,000 times the memory bandwidth”) ^clm-5326f7922809465cc3d2
- Thompson argues Cerebras chips suit inference, not training, but only while everything fits in on-chip memory; a larger model or KV cache makes them poor value, and whole-wafer yields hugely drive up cost. (§ Understanding Cerebras: “the moment you need more memory, whether that be for a larger model”) ^clm-01948bd50fb36c075a78
- Prediction: Thompson argues Cerebras' current pitch of fast tokens for coding is a temporary use case, while speed will matter lastingly where humans wait, such as voice on AI wearables. (§ Understanding Cerebras: “but I think this is a temporary use case”) ^clm-767ca957dd08474bd69c
- Thompson restates three LLM inflection points: ChatGPT showed token prediction was useful, o1 added reasoning where more tokens meant better answers, and Opus 4.5 with Claude Code brought the first usable agents. (§ Agentic Inference: “Opus 4.5 and Claude Code introduced the first usable agents”) ^clm-8b1ec7542ed0373fe7c9
- Thompson coins the split between answer inference (providing an answer) and agentic inference (doing a task), and says Cerebras targets answer inference while agentic inference will need an architecture unlike both Cerebras and GPUs. (§ Agentic Inference: “what I will call “answer inference” — and doing a task — what I will call “agentic inference.””) ^clm-e7b3dba4d8c3a8965bd2
- Prediction: Thompson argues the true power of agents is not doing work for humans but doing work without any human involvement, so coding's need for a human in the loop is temporary. (§ Agentic Inference: “they do work without human involvement at all”) ^clm-fae4622fde800995ef21
- Thompson argues token speed matters most for answer inference, but memory matters most for agentic inference, since agents need context, state, and history held in KV cache, host memory, SSDs, databases, and object stores. (§ Agentic Inference: “the most important aspect for agentic inference, however, is memory”) ^clm-3d24ff2bf45f6bc73d68
- Thompson argues that with no human in the loop, delays are fine, so slower and cheaper memory such as traditional DRAM makes more sense than HBM, and chips need not be cutting edge. (§ Agentic Inference: “slower and cheaper memory — like traditional DRAM, for example — makes a lot more sense”) ^clm-3114f56fe6122785b3c0
- Prediction: Thompson predicts Nvidia's architecture will likely keep dominating training, and that answer inference will be a meaningful but relatively small market where fast chips like Cerebras or Groq are very useful. (§ Agentic Inference: “Answer inference will be a meaningful market, albeit a relatively small one”) ^clm-895cfc39d2ecf3238c9f
- Prediction: Thompson predicts agentic inference will gradually unbundle the GPU, which strands HBM during prefill and compute during decode, in favor of high-capacity, lower-cost memory hierarchies with good-enough compute, where CPU speed for tool use matters more than GPU speed. (§ Agentic Inference: “Agentic inference will gradually unbundle the GPU”) ^clm-ff02535ae1e20260cd69
- Prediction: Thompson predicts agentic inference will be the largest market by far, because it is not limited by humans or time, and argues today's agents are just fancy answer inference. (§ Agentic Inference: “agentic inference will be the largest market by far”) ^clm-05cf088c008cfb451b3e
- Thompson argues that scaling with compute has implicitly meant Nvidia bullishness, but Nvidia's edge comes largely from latency, so if latency is not the key constraint its approach seems less worth a premium. (§ The Implications of Agentic Inference on Compute: “Nvidia’s approach seems less worth paying a premium for”) ^clm-b213042c1a5b496169c1
- Nvidia recognizes the shift: it launched Dynamo, an inference framework that splits up parts of inference, and ships standalone memory and CPU racks for larger KV caches and faster tool use, though Thompson expects hyperscalers to favor cost and simplicity. (§ The Implications of Agentic Inference on Compute: “helps disaggregate different parts of inference”) ^clm-7fd1c661cf9d29d13017
- Thompson argues China, despite lacking leading-edge compute, has everything agentic inference needs: good-enough GPUs and CPUs, DRAM, and hard drives; its gap is compute for training. (§ The Implications of Agentic Inference on Compute: “has everything it needs for agentic inference”) ^clm-ab7cb029d2f7cb3af2ac
- Thompson argues slower chips make space data centers more viable: offloaded memory lets chips run simpler and cooler, older nodes resist radiation better, use less power, and are more reliable for satellites that cannot be repaired. (§ The Implications of Agentic Inference on Compute: “slower chips actually make space data centers more viable”) ^clm-ca5653e80fa9a630e15f
- Jensen Huang regularly says Moore's Law is dead, meaning speed-ups will come from systems innovation; Thompson argues agents without humans may make Moore's Law not matter, because the compute we have is already good enough. (§ The Implications of Agentic Inference on Compute: “the compute we have is already good enough”) ^clm-d1c705e81458519544a6

## Entities

[[Anthropic|Anthropic]], [[Ben-Thompson|Ben Thompson]], [[Cerebras|Cerebras]], [[Groq|Groq]], [[Jensen-Huang|Jensen Huang]], [[Nvidia|Nvidia]], [[OpenAI|OpenAI]], [[SpaceX|SpaceX]], [[xAI|xAI]]

## Concepts

[[AI-Agents|AI Agents]], [[AI-Compute-Demand|AI Compute Demand vs Supply]], [[AI-Stack-Integration|Full-Stack AI Integration]], [[Answer-vs-Agentic-Inference|Answer Inference vs Agentic Inference]], [[Commodity-Cost-Advantage|Winning a Commodity Market on Cost]], [[LLM-Inflection-Points|Three LLM Inflection Points]]
