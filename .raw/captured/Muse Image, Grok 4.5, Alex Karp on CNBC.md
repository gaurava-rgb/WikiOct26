---
title: "Muse Image, Grok 4.5, Alex Karp on CNBC"
source: "https://stratechery.com/2026/muse-image-grok-4-5-alex-karp-on-cnbc/"
author:
published: 2026-07-09
created: 2026-07-24
description: "The battle for verifiable data is increasingly defining the AI race, from Meta to Grok to the frontier labs."
tags:
  - "clippings"
---
**Listen to this post:**

Good morning,

On [this week’s episode of Sharp China](https://sharpchina.fm/member/episode/a-missile-test-and-new-pla-generals-the-citic-plane-crash-americas-taiwan-interests-guo-wengui-jailed-and-ezra-jin-released), Andrew and Bill discuss Chinese missile tests, the CITIC plane crash, and America’s interest in preserving the Taiwan status quo.

Meanwhile, Jon at [Asianometry](https://asianometry.passport.online/member/episode/toto-from-toilets-to-e-chucks) produced [a video about one of my favorite companies](https://www.youtube.com/watch?v=CIB49e_r1OI): Toto. You know them and I love them for their toilets; they also happen to be indispensable to the AI supply chain.

On to the Update:

### Muse Image

From [Bloomberg](https://www.bloomberg.com/news/articles/2026-07-07/meta-debuts-new-ai-image-generation-model-inside-chatbot-instagram):

> Meta Platforms Inc. debuted a new image-generation artificial intelligence model, its first such release since the company spent billions to rebuild its AI lab under Chief AI Officer Alexandr Wang a year ago. The model, called Muse Image, is rolling out Tuesday inside the Meta AI chatbot, the company said in a blog post. It will also be embedded in Meta’s various social apps, including Instagram and WhatsApp. People can use it to generate images based on text prompts or by asking it to alter existing pictures. Advertisers, too, will soon have access to the model to create marketing materials. Users can also make images featuring friends or creators based on their publicly available Instagram posts, part of an effort by Meta to make the platform feel more personal. Those who don’t want others to “reuse or remix” their content using AI can opt out in the settings menu, according to the blog post.

The headline for Muse Image is exactly what Bloomberg leads with: end users have a new image model on Meta’s properties, and by all accounts it’s very good, thanks in part to incorporating many of the advancements that have transformed large language models. [Meta’s blog post about Muse Image](https://ai.meta.com/blog/introducing-muse-image-muse-video-msl/) detailed these features, including:

- Tool use, including coding (for things like plots, QR codes, interactive games, etc.) and search (for grounding images).
- Self-Refinement, which is Meta’s term for reasoning: the model iterates on images to correct mistakes and make them better.
- Test-Time Compute Scaling, which incorporates both of the first two items: the more compute you spend on an image the better it is.

What is most compelling, however, is the advertising angle; these were the headline takeaways from [Meta’s business blog](https://www.facebook.com/business/news/muse-image-for-businesses) (which, interestingly enough, still lives at a facebook.com URL):

> - In the coming weeks, Muse Image, the first image generation model from Meta Superintelligence Labs, will help power image generation in Meta Advantage+ creative — bringing smarter reasoning and iterative refinement to our popular gen AI ad creative tool.
> - Early results with Muse Image-powered generation variants show strong promise — advertisers who tested the experience cited higher-quality creative, with photorealism and product integrity standing out.
> - Muse Image now enables room restyling in Meta AI Shopping, letting people visualize products from your business’ catalog in their own spaces—creating a richer, more immersive path from discovery to purchase.

I’ve been talking for years about the obvious application of image generation to advertising: instead of creating 10 or 15 pieces of creative and A/B testing which ones work best, you will be able to have exponentially more possibilities that you can rank with a built-in scoring system — i.e. did the ad convert or not?

However, there is a deeper implication to this capability that was highlighted by Eric Seufert at [MobileDevMemo](https://mobiledevmemo.com/metas-muse-moat-integration-into-advantage/):

> More conceptually, Meta’s integration of its own ad platform tools with a foundation image generation model that it owns is an incredibly profound commercial advantage. There are immense benefits to proprietary model ownership for the purposes of establishing closed-loop creative optimization. The most obvious is that Meta is not dependent on an outside model provider whose access, pricing, roadmap, or availability could be limited or adversely changed by export controls, competitive pressure, or government intervention; see the case of Fable 5 and Mythos 5 for a recent relevant example of this.
> 
> But the more fundamental benefit of direct integration of Muse Image into Advantage+ is that Meta can train, tune, align, and evaluate its own model against domain-specific advertiser performance data that only it possesses, producing results that are more differentiated and more use-case-native than what could be achieved through fine-tuning a generic model. A foundation model can be trained in alignment with Meta’s own retrieval and ranking infrastructure, with output controls that differentiate its ad creative from that of standalone or other platforms’ tools, in ways that enforce brand safety and preserve product integrity, with latency and cost controls. These are enormously powerful advantages for an ad platform, and they sit at the heart of my argument over why Meta is reaping real rewards, now, through its AI investments.
> 
> Integrating Muse into Advantage+ is exactly the kind of narrative-supporting development that Meta should be pursuing to assuage investor anxiety over its AI investments; it is more visible, given the creative applicability, but it also showcases the power of foundation model ownership because an open weight model might have been fine-tuned for this use case instead (compare that to GEM, which is also a foundation model but for which no open weight alternative exists).

One of the single most important contributors to model improvement is verifiability. A major reason why coding has been such a fruitful area of AI development is because code is verifiable: does it work or not? That, by extension, means that the more that a particular task is verifiable, the faster it will be done by AI. Or, to put it another way, owning verification is extremely advantageous, and markets are verification mechanisms. Yes, you need to have enough liquidity to get sufficient signal — there is a *lot* of noise in this data — but that is exactly what Meta ads are: arguably the most liquid market in the world, with trillions of ads driving conversions or not. Any model that plugs directly into that signal is going to get better sooner.

### Grok 4.5

From [Bloomberg](https://www.bloomberg.com/news/articles/2026-07-08/spacexai-cursor-unveil-grok-ai-model-for-legal-finance-tasks):

> SpaceXAI has unveiled a new artificial intelligence model built in partnership with AI coding startup Cursor that’s meant to be more adept at finance, legal and coding tasks, in a bid by Elon Musk’s firm to gain ground on rivals like Anthropic PBC and OpenAI. The software, called Grok 4.5, marks the first joint AI model developed by the two companies and comes just weeks after SpaceX formally agreed to acquire Cursor in a deal that values the startup at $60 billion.

Grok 4.5 seems to be pretty decent; it’s also quite cheap relative to its performance; this is [Cursor Field CTO David Pan on X](https://x.com/davep/status/2074923005751533596):

![](https://x.com/i/status/2074923005751533596)

The benchmark on the left is Cursor’s own benchmark, so take the performance with the appropriate grain of salt, and frankly, it’s hard enough to convince people — including myself! — to even try other models once they’re used to a specific one, particularly if they use the associated harness, which is to say that Grok has a very long ways to go to actually win usage. What I’m not surprised by, however, is that the tie-up with Cursor is paying dividends. It’s a continuation of my point above: Cursor had and has a lot of usage and captured a ton of traces around code in particular, and it was always a good bet that that data would be exceptionally valuable.

What is worth noting is that this might also be another argument that OpenAI was ultimately harmed by the widespread consumer adoption of ChatGPT, at least absent a compelling advertising business: it’s not just that consumers were a distraction that didn’t subscribe enough even as they used a lot of GPUs, it’s that most consumer AI interactions aren’t particularly useful data for a feedback mechanism. This is in part due to the nature of chatbots — how do you know if the code you generated ran or not? — but also due to the fact that most people aren’t coding. They’re asking about recipes or life or who knows what else, many of which are, if not unanswerable, at least unverifiable.

### Alex Karp on CNBC

Last week Palantir CEO Alex Karp delivered [quite the interview on CNBC](https://www.cnbc.com/2026/07/01/palantir-karp-open-ai-anthropic-tokens.html), criticizing the leading model companies in particular. The video is a ride, and worth a watch, but there was one point he came back to again and again in an interview nominally about [Palantir’s deal to bring Nvidia’s open source Nemotron model to the U.S. government](https://blogs.nvidia.com/blog/palantir-secure-ai-us-agencies-nemotron-open-models/) (*excerpt lightly edited for clarity*):

> If you want to know how this came together from my perspective, there’s a lot of technical issues, the choice of who controls the models, who controls the weights, who controls the value of your business. But, you know, we’re sitting on critical infrastructure across America…and our clients are just \[so\] unhappy with the frontier labs…It’s like there’s just a level of discomfort and loss of trust…
> 
> The basic view among enterprises in this country is I’m going to chillax and waste my time with tokens. I’m going to get no value and they’re going to get my IP…They’re like, why would they get access to my data if they’re going to steal my alpha? Why wouldn’t I control the weights? That’s where you get this partnership. What aligns me with Nvidia and I think is what the most technical customers want, which is control over their compute, their models, their data stack and their alpha they want to know they own the means of production and it is not being transferred to someone else. They’re not interested in some fake deploy co that someone is deploying, and tokens that transfers the alpha to a third party.

Again later on:

> We need to rebuild trust and that trust is going to happen where everyone gets to ask and answer basic questions. Who owns the data? Where is it cached? Are the prompts secure? Is this being transferred to you?…What is the true cost? Not just what you’re paying. The true cost is not just what you make minus what you lose, meaning the value of your business. But we can get the the frontier application to be exactly the same, as a frontier model, without the risk of transferring the alpha of your business to a model. By the way, you could do this with a frontier model closed model too, but then the clients have to be able to ask and answer very basic questions. Are you keeping the data? Are you going to enter our business?
> 
> That’s my role, but I’m telling you in this country at every single enterprise I deal with. These people are livid. They’re like, I am paying for tokens that create no value. These people are stealing the weights and alpha of my business…and I can’t safely give it to an enterprise in this country without being certain that the alpha in the business could transfer to this model tomorrow, i.e. now I’ve got no business, no job.
> 
> **You sound pretty angry.**
> 
> This is the voice of American business that is being channeled through me, and I’m telling you it is absolutely a problem for this country.

What Karp is driving at is the flip-side of the points I am making above (and, I would add, is the same argument Microsoft CEO Satya Nadella made in [a recent Stratechery Interview](https://stratechery.com/2026/an-interview-with-microsoft-ceo-satya-nadella-about-finding-core-competencies/)): the challenge for enterprises when it comes to using the frontier models is not simply that tokens are expensive, but that they are potentially giving valuable data to the labs who, in the long run, have an economic imperative to move up the stack and own the customer directly.

This was already a concern, but I think the most underrated aspect of the Fable release was Anthropic changing the terms of service such that they would retain all data, even from enterprise customers — for safety reasons, of course. I wrote in [Anthropic’s Safety Superpower](https://stratechery.com/2026/anthropics-safety-superpower/):

> The models — not even Mythos — are not yet at this point. What they need, beyond more compute, is more and better data. Model improvements increasingly come from reinforcement learning; some of this can be generated synthetically, but the most powerful lever for a frontier lab is real world use.
> 
> This, I think, is a major reason why both OpenAI and Anthropic offer their heavily subsidized subscription plans. SemiAnalysis [recently estimated](https://x.com/SemiAnalysis_/status/2064815044085318040) that a $200 plan gets you $8,000 worth of Claude tokens and $14,000 worth of Codex tokens. Of course both are fighting for user and developer mindshare, but they’re also fighting to have access to actual usage data to make their models better.
> 
> Anthropic upped the ante in a major way with Fable, announcing that they would retain the data for all usage for 30 days, even for their enterprise plans that previously promised zero data retention. The company said they would not train on this data, but they didn’t put in any sort of safeguards to guarantee they wouldn’t do so in the future (like storing the data with a third party). If this policy change (whenever Fable is restored) doesn’t lead to a significant loss of customers, I suspect it’s only a matter of time until they start using the data: it’s simply too valuable to their end goals.
> 
> Note also the virtuous cycle with moving up into user touchpoints: the more workflows that are done directly with Claude or Codex, the more data each company gets to feed back into their training, which makes their products that much more capable and useful, expanding the number of workflows they can serve, expanding their access to data.

To take this full circle, this is another reason to be a bit bullish about Meta: they operate in markets where it is a given that Meta gets and acts on all of the data; they don’t need to fight enterprise data policies. Anthropic, meanwhile, appears to be making a bet that they can be better enough that they can get the data they need anyways (and that said data will drive that virtuous cycle where their offering improves that much more rapidly); they might cash it in.

---

This Update is also available as a podcast. To receive it in your podcast player, [visit Stratechery](https://stratechery.passport.online/member).

The Stratechery Update is intended for a single recipient, but occasional forwarding is totally fine! If you would like to order multiple subscriptions for your team with a group discount (minimum 5), please contact me directly.

Thanks for being a subscriber, and have a great day!