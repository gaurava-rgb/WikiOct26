---
title: "Nvidia Earnings, The AI Stack, Nvidia’s New Reporting"
source: "https://stratechery.com/2026/nvidia-earnings-the-ai-stack-nvidias-new-reporting/"
author:
published: 2026-05-26
created: 2026-05-27
description: "Nvidia is changing its reporting to delineate between hyperscaler sales — where Nvidia is fighting commoditization — and everyone else, where Nvidia runs the whole stack."
tags:
  - "clippings"
---
**Listen to this post:**

Good morning,

On [Thursday’s episode of Sharp Tech](https://sharptech.fm/member/episode/much-ado-about-data-centers-what-tech-gets-wrong-about-its-critics-q-a-on-space-x-chinese-ai-elon-musk), Andrew and I discussed the burgeoning opposition to data centers.

In addition, former Senator Ben Sasse, who was [diagnosed with Stage 4 pancreatic cancer](https://www.nytimes.com/2026/04/09/opinion/ben-sasse-death-pancreatic-cancer.html), launched a podcast earlier this year with Chris Stirewalt called [Not Dead Yet](https://www.spreaker.com/podcast/not-dead-yet--6881632); I was honored to be a guest on [the most recent episode](https://www.spreaker.com/episode/ben-thompson--72062990).

On to the Update:

### Nvidia Earnings

From the [Wall Street Journal](https://www.wsj.com/tech/ai/nvidia-nvda-1st-quarter-earnings-report-2026-stock-c2bb9c1c):

> Chip giant Nvidia reported record sales and income Wednesday, driven by surging demand for data-center computing and the astronomical rise of artificial-intelligence agents. Sales for the April quarter reached $81.6 billion, up 85% from the year-earlier period and beating the $78.9 billion that analysts polled by FactSet had forecast by 3.4%. Net income was $58.3 billion for the quarter, more than three times the year-earlier result and 36.5% higher than the $42.9 billion analysts had predicted. “Demand has gone parabolic,” Chief Executive Jensen Huang said in a conference call with analysts. “The reason is simple: The era of agentic AI is here.”
> 
> The record-high sales were driven by growth in Nvidia’s data-center segment, especially the sale of computing hardware, which includes the company’s graphics processing units, or GPUs, as well as other chips. Sales of networking hardware tripled from a year ago to a record $14.8 billion. The company also announced two shareholder-friendly changes: an $80 billion share buyback plan and an increase in the company’s quarterly cash dividend from one penny a share to 25 cents. Chief Financial Officer Colette Kress said in a conference call that the company intends to return 50% of its free cash flow this year to shareholders.

Nvidia’s earnings were, as you would expect in a supply-constrained world, fairly predictable. The company continues to crush it, and notably, is significantly increasing the commitment it is making to shareholders in terms of returning cash via both dividends and stock buybacks.

One interesting wrinkle is the way that the company talked about the explosion in revenue from the frontier labs. CFO Colette Kress in [her prepared remarks](https://seekingalpha.com/article/4907259-nvidia-corporation-nvda-q1-2027-earnings-call-transcript) called out Codex as a driver:

> There are 2 primary drivers behind the accelerating build-out of AI infrastructure. First, from search and advertising to recommender systems and content understanding. The largest hyperscale workloads continue to transition from CPU to GPU-based accelerating computing. Second, the adoption of products and services native to AI is inflecting. Since the advent of ChatGPT, we have witnessed mainstream AI transition from one-shot inference to reasoning and to now agentic. AI is no longer a nice to have. AI is now a necessity for enhancing productivity across all industries and roles. This is propelling revenue acceleration across all layers of the AI cake, including energy, chips, infrastructure, models and applications. Growth in the model layer, particularly at Anthropic and OpenAI has been incredible with momentum continuing to accelerate, including breakout growth in OpenAI’s Codex since the launch of GPT-5.5.

The distinction here is that while [OpenAI recently announced a deal to run on Trainium](https://stratechery.com/2026/an-interview-with-openai-ceo-sam-altman-and-aws-ceo-matt-garman-about-bedrock-managed-agents/), for now all of their training and inference run on Nvidia chips, ergo, if OpenAI models are being used more, then Nvidia chips are being used more.

Anthropic is actually the exact opposite; Huang noted that Nvidia’s “coverage of Anthropic has been largely zero until just recently”, thanks to the fact that Anthropic got investment from Google and Amazon in exchange for running on TPUs and Trainium, but that that is in the process of changing rapidly:

> We are growing share in inference, and we’re growing share in inference very, very quickly. And the reason for that is this year, the number of frontier model companies grew. And so there’s Cursor and Perplexity and there’s some new model companies, TML and Reflection, and the list goes on. And so the number of frontier model companies has grown, and we added Anthropic to our partnership this year. They’re expanding incredibly fast. We’ve partnered with them to secure computing capacity across Azure, AWS, CoreWeave. I forget who else we’ve already announced, but there’s a whole list of others that we are bringing online for them. And so the amount of capacity that we’re going to bring online for Anthropic this year and next year is going to be quite significant, very significant.

This has probably been an under-appreciated bullish factor for Nvidia: the company has been growing as it has without being a part of the growth of the fastest growing lab. At the same time, that also reinforces that Nvidia’s position in the AI stack is not unassailable.

### The AI Stack

The AI Stack looks something like this, starting from the bottom:

- Semiconductor equipment makers
- Logic fabs
- Packaging
- Memory fabs
- Chip makers
- Networking
- Data centers
- Model makers
- Applications
- Users

In the short run, as long as there are shortages, there is money to be made at every level of the stack; in the long run, once supply and demand come into balance, the most value accrues to whoever in the stack is able to integrate around a bottleneck in the stack and commoditize everyone else.

Nvidia’s traditional moat has been CUDA, which binds developers to its chips; most AI developers, however, are operating at a level of abstraction where CUDA doesn’t matter. CUDA does matter to model makers, but Anthropic (and Google) has already demonstrated that it’s not essential when it comes to training and serving a leading edge model.

Another Nvidia moat, at least for the short to medium-term, is that the company is first-in-line for supply, particularly from logic fabs (TSMC), packaging (TSMC), and memory. Again, however, this is not a sustainable source of value capture in the very long run, as more supply comes online.

A third Nvidia moat is that the company also sells networking specifically, and systems broadly; Huang said on the call:

> We built the Nvidia compute platform over 3 decades, one architecture, vast ecosystem, extreme co-design across chips, systems, networking and software. We built it ahead of this moment so that when agentic AI arrived, Nvidia would be ready. It has arrived.

Nvidia isn’t just ready for the AI moment: they’re also ready to defend their position in the stack, which leads to what was by far the most interesting part of these earnings — and the surest sign that I (and by extension all of you) really am a business model nerd: Nvidia changed their reporting.

### Nvidia’s New Reporting

Here was Kress’s introduction of the new numbers:

> Before we deep dive into Data Center, we’d like to brief you on our transition to a new reporting framework that better reflects our current and future growth drivers. We have 2 market platforms, Data Center and Edge Computing. Within Data Center, we will report 2 submarkets: hyperscale and ACIE, which incorporates AI Clouds, Industrial and Enterprise. Hyperscale will include revenue from the public cloud and the world’s largest consumer Internet companies, while ACIE addresses our growth opportunities in diverse AI purpose-built data centers and AI factories across industries and countries.

Hyperscalers are, from Nvidia’s perspective, frenemies: on one hand, they’re a big part of the business — 50% of Data Center revenues. On the other hand, it is the hyperscalers who are both the most interested in and the most capable of reducing Nvidia to just a chip maker. And, if Nvidia is just a chip maker, their long run ability to extract revenue from the value chain is compromised. You see this most directly in the hyperscalers’ diligence in making their own chips, but also in terms of forcing Nvidia chips into their own networking solutions.

To that end, I think the driving motivation behind this change was to break out the new ACIE submarket: these are datacenters that need the full Nvidia stack, which is to say they are datacenters that, in the long run, will consistently allow Nvidia to capture outsized value in the stack. Huang explained why these were Nvidia’s best customers:

> The second category is all of the AI native clouds. They’re regional, they’re all over the place, they’re start-ups all over the world, supporting those companies. They’re enterprise, 250,000 enterprise companies around the world, many of them will have to build or want to build AI factories for themselves to operate. Many industrial companies, there’s no choice but to put the computer where the context is, where the action is, you can’t put that in the cloud. It has to respond reliably, quickly every single time, can’t imagine a chip plant, a chip fab being connected to a cloud service provider, doesn’t make any sense. And so the second category and the sovereign AI clouds. And so there’s a whole category of data centers that semi-custom chips just don’t apply because these data centers want to buy systems, they want to operate systems, they don’t want to design, they don’t want to build it themselves…
> 
> The second cluster is growing incredibly fast. Our share of that, of course, is very, very large. We’re fairly unique in our ability to be able to serve this industry. Our platform is built like it’s vertically integrated so that everything works but when — then we disassemble it, so that people could build and buy it in the configuration they want and assemble it the way they like. And so this second category is fairly poorly understood because there are just so many small companies — or so many companies and each one of the installations are relatively small compared to, of course, one of the hyperscalers. And so if you look at the segmentation and the size of each, you could see that, in fact, we’re growing share in the hyperscalers because we now have much bigger support from Anthropic, a new partner of ours, and we’re helping them expand their capacity greatly in the coming years. And then the second, very few companies have exposure into the second category because of the platform solution that we have.

Another way to explain this segment is that it is, at least relative to the hyperscalers, already commoditized. A random data center or enterprise customer is not going to make their own chip or roll their own networking; they’re just going to buy entire systems from Nvidia, and Nvidia really doesn’t have any competition in this space. Moreover, as long as demand exceeds supply, Nvidia can continue to ensure that this category gets as much allocation as they can handle. To that end, this segment’s share of Nvidia sales has been increasing over the last year (the chart shows the last 9 quarters):

![](https://i0.wp.com/stratechery.com/wp-content/uploads/2026/05/nvidia-1.png?w=1330&ssl=1)

It’s interesting to consider whether or not this is a good trend for Nvidia. The bearish take is that Nvidia’s position in the hyperscalers — it’s most direct competitor for value in the AI stack — is in fact threatened, leading to a shrinking share of sales; the bullish take is that Nvidia’s push to build out neoclouds and enterprise is working, and that the company is enabling customers who will be locked in not just for chips but for networking and all-up systems — with their attendant high margins — for a long time to come.

Given the fact we are still operating in a supply-constrained world, which is another way of saying we are operating in a world where Nvidia can pick-and-choose who to sell to, I think this trend is bullish. Yes, Nvidia has very large dependencies on the hyperscalers who are doing everything they can to design around Nvidia, even as they need to buy more; however, a full 50% of their business is now elsewhere, and every point of share that is elsewhere is not just an indicator of current Nvidia sales but also lock-in for future sales.

That noted, this isn’t necessarily *resilience* in terms of diversifying demand: a huge amount of the neocloud capacity is actually just going to serve the hyperscalers, and ultimately, the frontier labs. It’s just a play — and this reporting change an advertisement — for Nvidia’s ability to leverage demand into long-term lock-in.

ACIE, I would add, is almost certainly the core of the addressable market for Vera CPUs, which was the other big talking point on the call. Kress said:

> Building on the success of our Grace CPU, Vera is arriving just in time to meet this inflection. Built on custom ARM cores and codesigned end-to-end with Rubin GPUs and NVLink, Vera will deliver up to 1.5x faster performance per core, 2x performance per watt and 4x density per rack compared to x86-based alternatives. Vera CPU opens a brand-new $200 billion TAM for Nvidia, a market we have never addressed before, and every major hyperscale and system maker is partnering with us to get it deployed. We have visibility to nearly $20 billion in total CPU revenue this year, setting us up to become the world’s leading CPU supplier.

$20 billion in revenue — as amazing as that would be! — would not make Nvidia the largest CPU maker; I interpret the last clause as referring to the long run. Regardless, while Kress talks about selling to hyperscalers, the far more obvious customers are the ACIE category, particularly the neoclouds: they are already all in on Nvidia, while hyperscalers also have their own custom CPU programs, as well as long-running relationships with AMD and Intel.

That, by extension, adds one more bit of context to the chart above: a 50/50 split in revenue between hyperscalers and ACIE almost certainly implies far more units to the former; the latter is buying a lot more equipment from Nvidia than just chips, and likely paying more for the privilege given they are a captive customer base (thus the base that is interested in Vera CPUs). You can certainly see why Nvidia has gone to so much trouble to make it a viable category.

---

This Update will be available as a podcast later today. To receive it in your podcast player, [visit Stratechery](https://stratechery.passport.online/member).

The Stratechery Update is intended for a single recipient, but occasional forwarding is totally fine! If you would like to order multiple subscriptions for your team with a group discount (minimum 5), please contact me directly.

Thanks for being a subscriber, and have a great day!