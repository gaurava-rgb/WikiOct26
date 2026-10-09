---
type: concept
title: Local Inference (Running AI Models on Your Own Hardware)
status: developing
created: 2026-09-29
updated: 2026-10-09
tags:
  - concept
source_count: 6
---

# Local Inference (Running AI Models on Your Own Hardware)

Running an AI model on computers you own instead of paying a cloud provider like Anthropic or OpenAI per request. You pay up front for hardware (mostly GPU memory, called VRAM, which sets how big a model fits), then each use is nearly free and your data never leaves your machine. Open weight models (models whose files anyone can download) make it possible; the trade-off is cost, setup work, and models a step behind the best hosted ones.

## Evidence by source

### 2026-07-05 [[2026-07-05-jamesob-local-llm-Running-LLMs-Locally|jamesob/local-llm: Everything I know about running LLMs locally]]

- jamesob pitches local AI as an answer to dependence on the big labs, saying that if Dario Amodei and Sam Altman give you heartburn, they should. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-e846a64f99d35b12dff1|cite]])
- jamesob says about $2k buys two RTX 3090 GPUs with 48GB of GPU memory in total, enough to run the Qwen3.6-27B model, which he calls awesome. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-6c52609d4f94c6922a5c|cite]])
- jamesob says about $40k buys the next step up in model intelligence, something he rates as pretty close to Claude Opus. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-878821e35fa30cedf803|cite]])
- At the $40k level, jamesob's pick is four RTX PRO 6000 GPUs for 384GB of GPU memory in total. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-18f0f7cca2bb19b008f8|cite]])
- jamesob names a compressed 594-billion-parameter GLM-5.2 model as the best model for four RTX PRO 6000s as of July 2026, served at about 80 tokens per second with a 460k-token context window. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-e870c97e7d499849a009|cite]])
- jamesob's four RTX PRO 6000 Blackwell GPUs (96GB each) cost about $46,000, which is where most of the money went. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-a0d79b5725dabcd2b634|cite]])
- Because computer memory had become so expensive, jamesob built a last-generation DDR4 system from eBay parts to host the GPUs and keep the base system cheap. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-e9938f1176fe8490822d|cite]])
- jamesob says a new PCIe5 and DDR5 base system was terrifically expensive as of July 2026, so he spent on GPU memory, where it counts, instead. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-adfc9d79876f6b3c38dd|cite]])
- jamesob's base system, a last-generation AMD EPYC Milan server with 128GB of DDR4 memory, cost $5,587 in parts, mostly from eBay. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-02a6b96d2b1d8d435189|cite]])
- jamesob used PCIe Gen4 switches from indie maker c-payne so the GPUs can exchange data directly at wire speed, cutting latency without costly PCIe5 hardware. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-8fe7547a5cf7ed4c4f62|cite]])
- jamesob stores all model weights on a mirrored ZFS filesystem across two 8TB drives, downloads them from Hugging Face, and runs each model in its own Docker container. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-db789676df03e09214a4|cite]])
- jamesob argues a key to making open source models good is tooling them properly, giving his agent web search, a Telegram bot for alerts, and a private Gitea code server. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-13b9be0c56d326325251|cite]])
- jamesob finds local speech-to-text with whisper-large-v3 surprisingly useful and says he feels comfortable using it, unlike a hosted equivalent; it needs only about 11GB of GPU memory. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-5813fb78ba7f869dd5e1|cite]])
- jamesob suggests an alternative: a linked cluster of four DGX Spark machines with 512GB of memory as a slow, big brain driving a small Qwen model for quick rote tasks. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-cd318b4424d21569c346|cite]])

### 2026-09-10 [[2026-09-10-The-iPhone-Duo-The-Intelligent-Personal-Hub-Apple-Watch-Audio-Intelligence|The iPhone Duo, The Intelligent Personal Hub, Apple Watch Audio Intelligence]]

- Thompson accepts the intelligent personal hub framing but notes Ternus' description conveniently matches the iPhone, and argues an iPhone, however powerful, is fundamentally less capable than something running in the cloud. ([[2026-09-10-The-iPhone-Duo-The-Intelligent-Personal-Hub-Apple-Watch-Audio-Intelligence#^clm-f96fb0f453a2ef6dcc33|cite]])
- Thompson argues that using powerful cloud models for everything will be more intelligent than Apple's approach of carefully rationed fallbacks to on-device models. ([[2026-09-10-The-iPhone-Duo-The-Intelligent-Personal-Hub-Apple-Watch-Audio-Intelligence#^clm-d2a9aefb5abab2f50f28|cite]])

### 2026-09-14 [[2026-09-14-Anthropic-Data-Fears-Prompt-Nvidia-Palantir-and-Booz-Allen-to-Restrict-Model-Use|Anthropic Data Fears Prompt Nvidia, Palantir and Booz Allen to Restrict Model Use]]

- Nvidia uses Fable only for less sensitive work such as open-source projects and runs sensitive work, like AI supply chain monitoring, on its own Nemotron models. ([[2026-09-14-Anthropic-Data-Fears-Prompt-Nvidia-Palantir-and-Booz-Allen-to-Restrict-Model-Use#^clm-3aafd5013488f2437bc6|cite]])
- Northrop Grumman runs open-source models on air-gapped servers for coding and research, using models from Poolside, Luminary and Nvidia. ([[2026-09-14-Anthropic-Data-Fears-Prompt-Nvidia-Palantir-and-Booz-Allen-to-Restrict-Model-Use#^clm-f27035b360b75fadae28|cite]])

### 2026-09-16 [[2026-09-16-Apple-Considers-Return-to-Server-Market-Has-Talked-With-Nvidia-to-Use-Network-Tech|Apple Considers Return to Server Market, Has Talked With Nvidia to Use Network Tech]]

- Over the past year large AI labs bought tens of thousands of Mac minis and Mac Studios, causing an extreme shortage. ([[2026-09-16-Apple-Considers-Return-to-Server-Market-Has-Talked-With-Nvidia-to-Use-Network-Tech#^clm-96f74139d5a6f7903ebb|cite]])

### 2026-10-07 [[2026-10-07-AIs-Simmering-Question-Where-Is-All-the-Automation|AI's Simmering Question: "Where the F--- Is All the Automation?"]]

- Microsoft unveiled a push to run AI on Windows PCs instead of the cloud, which it says cuts customer costs. ([[2026-10-07-AIs-Simmering-Question-Where-Is-All-the-Automation#^clm-631062491567b1e7230a|cite]])

### 2026-10-07 [[2026-10-07-Where-Nvidias-100-Billion-Dealmaking-Juggernaut-Will-Go-Next|Where Nvidia's $100 Billion Dealmaking Juggernaut Will Go Next]]

- Prediction: Nvidia's next deal targets are expected to be robotics, self-driving technology, and AI models that run locally on phones and home computers, per bankers, lawyers and investors who have worked with it. ([[2026-10-07-Where-Nvidias-100-Billion-Dealmaking-Juggernaut-Will-Go-Next#^clm-afea99a0c5c8bc59b578|cite]])
