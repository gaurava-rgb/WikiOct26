---
title: "Neocloud Prime Intellect Acquires Startup To Speed Up Inference"
author: Stephanie Palazzolo
publication: The Information
published: 2026-10-13
url: https://www.theinformation.com/articles/neocloud-prime-intellect-acquires-startup-speed-inference
kind: reading-notes
note: "Paraphrased notes with short quotes, taken from Gaurav's subscription. Not the full article text."
---

# Notes: Neocloud Prime Intellect Acquires Startup To Speed Up Inference

The Information, Stephanie Palazzolo, 2026-10-13 (AI Agenda newsletter).

## The deal

- Neoclouds (newer GPU cloud companies, not the big three hyperscalers) and inference providers that help app developers run open-source models are trying to stand out in a very crowded market.
- Prime Intellect, a San Francisco neocloud valued at $1 billion in an equity financing in July 2026, is buying a startup to make open models run faster and cheaper on its Nvidia servers than at rivals.
- The target is Moondream, a young open-source model developer with fewer than 10 employees, per Prime Intellect co-founder and CEO Vincent Weisser.
- Weisser would not share the deal terms. Moondream has raised $4.5 million in funding.

## What Moondream brings

- Moondream, based in San Francisco and Seattle, is best known for an open-source vision-language model that understands images, such as spotting boxes in a warehouse photo or ads in a livestream.
- But Prime Intellect is mainly buying it for its staff's skill at writing software that makes models run more efficiently, Weisser said.
- Moondream's staff know "megakernels": a way to speed up inference by fusing many separate math operations on a GPU into one continuous operation. This cuts GPU idle time between tasks.
- Moondream has built a compiler (software that turns model code into GPU instructions) that can generate megakernels for many models, the startup has said.
- That compiler and Photon, Moondream's proprietary tech for running models fast, will be folded into Prime Intellect's tech, Weisser said.
- Megakernels are not new: Together AI has also written about its megakernel work. But engineers say writing them has been a manual process, while Moondream says its compiler works largely automatically.

## New customers beyond text

- Moondream's experience optimizing non-text models, like image models, is relatively rare in an industry hyper-focused on text AI, Weisser said.
- Prime Intellect hopes the talent helps it serve customers building AI for robotics and computer-using AI agents.
- Those customers are not well served by other neoclouds and inference providers today and could be new revenue sources.

## How big Prime Intellect is

- Prime Intellect said in July 2026 it had passed $100 million in annualized revenue (one month's revenue times 12), implying a little over $8 million a month at the time.
- That is much smaller than Fal, at more than $800 million in annualized revenue, or Together AI, at over $1 billion.
- Besides running models and selling compute for training and inference, Prime Intellect sells software for post-training, also called reinforcement learning: tuning models on user and customer feedback.
- It has also trained its own models and built other AI software, such as coding and AI research agents.
- After the OpenAI revenue confusion the week before, the newsletter says it was assured these annualized figures are real.
- Many inference providers pay a large share of revenue to the cloud firms that own the servers. Prime Intellect is different: it operates its own hardware.

## AI Deep Dive: Goodfire's Tom McGrath

- Tom McGrath, chief scientist of Goodfire AI, a startup focused on mechanistic interpretability (explaining how AI models work inside), says AI could automate that field quickly.
- Quote: "Of all the fields of science, interpretability should be the one that gets most revolutionized," or revolutionized first, by AI.
- His reasoning: unlike pure math, done mostly on paper, interpretability is like biology, where experiments must be run and data collected; AI research agents could run many of those experiments.
- He wants to deploy "the swarm" of AI agents to produce orders of magnitude more experimental data and use it to improve scientific understanding.

## Deals and news roundup (selected)

- Microsoft is overhauling leadership of its Azure cloud business, cloud chief Scott Guthrie told staff Monday, as it consolidates units and reorients around AI.
- NTT Data is in final talks to build Anthropic's first dedicated data center in Japan: an Osaka facility with power intake of up to 500 megawatts that could cost up to ¥1 trillion ($6.3 billion), among the largest such projects in Japan.
- JPMorgan and Goldman Sachs, leading a $5 billion loan sale for Volta Infrastructure Holdings, underwrote a $1.3 billion term loan themselves rather than a separate $3.7 billion loan for GPU purchases.
- Tencent is preparing to raise at least $4.5 billion through US dollar and offshore yuan bonds, mainly to fund AI capital spending, chiefly chips.
- SWI Group, which controls former FTX-owned bitcoin miner Genesis Digital Assets, raised €800 million ($894 million) at a €6.1 billion valuation to convert mining sites into AI data centers in Europe and the US.
- CrowdStrike is in advanced talks to buy Israeli startup Orion Security, whose AI agents flag corporate data leaks, for about $500 million.
- Winverse AI, a stealth Chinese robot AI startup, is in talks to raise tens of millions of dollars in a seed round led by DeepSeek.
- Salesforce agreed to buy Israeli startup Loops, whose AI explains why business metrics change, for an estimated $30 million.
- Character.ai filed for Chapter 11 bankruptcy (a US court process to reorganize debts) and agreed a deal where a Walt Disney affiliate pays $20 million for a non-exclusive license to some of its IP and provides transition services using former Character.ai staff Disney hired.
- Meta unveiled two new AI models, Muse Wonder and Muse Wonder Full, on Monday.
- Microsoft announced the Maia 300, its latest homegrown AI chip, and plans "multi-gigawatt deployments" of it starting next year.
- Others: Suki raised $90 million (Series E, medical documentation AI); Ambi raised $26 million; Empirical Machines in talks for $15 million seed at about $80 million valuation; Zhejiang Sankai raised over $70 million (robot gear reducers).

## Why it matters for the wiki

- AI shift 2024-2026 story: inference providers are fighting on software efficiency (megakernels, compilers) and on owning hardware, not only on renting GPUs.
- Anthropic journey: a first dedicated Japan data center of up to 500 MW extends its push to own or lease its own capacity.
- Nvidia journey: neoclouds like Prime Intellect run Nvidia servers and compete by squeezing more out of each GPU.
- Meta journey: Muse Wonder and Muse Wonder Full extend the Muse model line.
- OpenAI journey: the annualized revenue caveat follows the OpenAI ARR mix-up the week before.
