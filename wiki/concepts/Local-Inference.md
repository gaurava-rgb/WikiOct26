---
type: concept
title: Local Inference (Running AI Models on Your Own Hardware)
status: developing
created: 2026-09-29
updated: 2026-10-13
tags:
  - concept
source_count: 7
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

### 2026-10-10 [[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes|GPUs in the Wine Cellar: Why Techies Are Hoarding AI Compute in Their Homes]]

- Former Microsoft executive Gary Flake built a home computer with seven Nvidia GPUs from discounted parts for under $6,000 to train AI models on terabytes of brain-scan (EEG) data. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-aa19f4786540bd177cfa|cite]])
- Flake says owning the machine beat paying AWS or Microsoft monthly cloud fees, even after $10,000 to $20,000 of electrical upgrades and a new cooling system to handle its heat. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-605d52746fad376287c2|cite]])
- Gary Flake summed up his choice to run AI on his own hardware: I want to own. I don't want to rent. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-dad52f48b3f6d6153303|cite]])
- The Information says running AI in attics, basements and home offices is an unexpected outcome of the AI boom, while leading AI firms run models in data centers with tens of thousands of GPUs. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-7256df866c5a353f6878|cite]])
- A growing local AI movement of small developers and tinkerers runs AI on their own computers for cost, privacy and convenience, and some libertarian-minded developers see it as a guard against governments cutting off access. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-c21986d73b9b6f2c73a8|cite]])
- Autonomous agent platforms like OpenClaw, which work with a user's local apps and files, helped fuel the home AI movement. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-dba8ac85ff9d7aca17f9|cite]])
- In September 2026 Shopify CEO Tobi Lütke went viral with a photo of three racks of AI gear in his Toronto wine cellar, including a Dell computer with an Nvidia GPU marketed as the ultimate deskside supercomputer. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-3399b95c98f4ff41d3c5|cite]])
- As of October 2026 Apple is seeing booming sales of its Mac mini and Mac Studio, both favorites of AI agent developers running machines at home. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-9340c5a0271c016edb71|cite]])
- Dell says it sees huge growth from the home AI community, and Dell engineer Marc Hammons said sales grew explosively after OpenClaw appeared earlier in 2026. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-4c5df0f705cfd29eaa4b|cite]])
- Crazy Egg CEO Hiten Shah, who mined Ethereum on eight home GPUs in 2020, now runs 18 computers at home for AI development, including 14 Mac minis and Mac Studios. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-89bbcbc153d8e4b8e1e8|cite]])
- Hiten Shah says local compute gives him more control over his software's performance because cloud AI models suffer outages and slowdowns, and models get janky for days after each new cloud release. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-a8a377fcfa5eae76808a|cite]])
- Heat is the hidden cost of home AI rigs: Hiten Shah's home office sometimes reaches 85 degrees Fahrenheit from his machines. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-0deeaf3805c3fe13e9ff|cite]])
- The YouTuber Digital Spaceport runs a garage home data center with five AMD GPUs, running Alibaba's open model Qwen 3.8 27B to edit and analyze his videos. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-dc478aa8b6b3f0f993f3|cite]])
- YouTuber 0xSero moved his four Nvidia 6000 GPUs from his home office to the attic in Poland because they were noisy and ran so hot they dried out the room. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-6ca746675e402bb5befd|cite]])
- 0xSero says Cursor raising its prices in late 2024 was the moment he decided to switch from cloud AI to local AI. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-e5827b0d2bf5e01792a3|cite]])
- 0xSero argues people should own and control their AI systems because governments may one day try to restrict access to the technology. ([[2026-10-10-GPUs-in-the-Wine-Cellar-Why-Techies-Are-Hoarding-AI-Compute-in-Their-Homes#^clm-3f50f3682fac2df96006|cite]])
