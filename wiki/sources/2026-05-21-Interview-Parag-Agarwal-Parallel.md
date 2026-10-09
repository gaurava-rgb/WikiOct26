---
type: source
title: An Interview with Parallel Founder Parag Agarwal About Valuing Content on the Agentic Web
status: evergreen
created: 2026-09-29
updated: 2026-09-29
tags:
  - source
  - source/interview
author: Ben Thompson
published: 2026-05-21
publisher: Stratechery
url: "https://stratechery.com/2026/an-interview-with-parallel-founder-parag-agarwal-about-valuing-content-on-the-agentic-web/"
raw: .raw/captured/An Interview with Parallel Founder Parag Agarwal About Valuing Content on the Agentic Web.md
source_id: src-3aa7b1e3c6445b375cd5
---

# An Interview with Parallel Founder Parag Agarwal About Valuing Content on the Agentic Web

Ben Thompson, Stratechery, published 2026-05-21.

## Summary

Ben Thompson talks with Parag Agarwal, the former Twitter CEO who now runs Parallel, a search engine built for AI agents. Agarwal argues that agents will use the web far more than people, but they do not see ads, so the money that paid for web content will dry up. Parallel's answer is Index, which estimates how much each source helped an agent's paid work using a game theory tool called Shapley values, then pays content owners from a shared pool. It matters because it is one of the first concrete attempts to price content for agents, and its early data rewards unique facts like local news over widely copied analysis.

## Key claims

- Parallel, founded by Parag Agarwal in 2023, is a search engine for AI agents that mixes compute, models, and search, and delivers results based on how much the customer is willing to spend. (“Parallel is a search engine for AI agents, using a combination of compute, models, and search”) ^clm-c173324ef5a87661668d
- In the week of May 21, 2026, Parallel launched Index by Parallel, which shows what the content on any given site is worth to agents and pays content creators based on that value. (“which shows what the content on any given site on the web is worth to agents”) ^clm-a44560fb776c5d3413a4
- Agarwal says he joined Twitter as its most junior software engineer, because he loved the product. (§ Twitter: “I ended up at Twitter as the most junior software engineer at the time”) ^clm-8ae04bc583aee5e0a72d
- Agarwal says Twitter's ads team grew revenue from almost nothing to a couple billion dollars in a couple of years after going public. (§ Twitter: “we grew revenue from like nothing to a couple billion dollars in a couple of years”) ^clm-cf8467de9bb5bd6e9be0
- Agarwal says that after the IPO, Twitter's own projections showed it would stall at about 90 million daily active users (DAU, people who use it each day), so he moved from ads to the consumer product. (§ Twitter: “Twitter was going to saturate out at about like 90 million or so DAU”) ^clm-230b9bacefff082fd8c5
- Agarwal says bringing machine learning into Twitter's feed, against internal resistance, restarted DAU growth within months. (§ Twitter: “within months, we were able to show that you can actually re-energize Twitter’s growth”) ^clm-aa7b14a235cb2e269076
- Agarwal calls Bluesky, the decentralized protocol effort he worked on under Jack Dorsey at Twitter, a failure. (§ Twitter: “It didn’t turn out the way I had hoped — I’d call that a failure”) ^clm-534f32f4f7eeb176bbed
- Agarwal says that as CEO during the Elon Musk takeover, he was already working with the board on a meaningful layoff, though smaller than the one Musk later made. (§ Twitter: “I was working with our team and board to do a meaningful layoff, not as big as that eventually happened”) ^clm-016885738db9b30c3dc7
- Agarwal says his biggest regret is not building a materially better Twitter business during his years as CTO, and he shares the blame with Jack Dorsey. (§ Twitter: “The years when I was the CTO I would build a materially better business”) ^clm-45d2c43eab8d08da315c
- Agarwal explains Shapley values with a gloves example: with one seller of a left glove and two sellers of a right glove, the Shapley math pays about 4x more for the scarce left glove. (§ Shapley Values: “you’d roughly end up paying them 4x for the left glove that you pay for the right glove”) ^clm-f36d1a0b6c73fdf47279
- Prediction: Agarwal says that three years ago he became convinced agents will use the web 1000x more than humans ever have. (§ Shapley Values: “I got obsessed that agents will use the web 1000x more than humans ever have”) ^clm-3ba8477483de4dcadd8f
- Agarwal argues the web runs on three business models, subscriptions, advertising, and transactions, and the first two depend on human attention, which agents do not supply, so a new model is needed. (§ Shapley Values: “If humans are not showing up as traffic reading pages, those are not going to drive the web”) ^clm-86a9b1378b74a6c9cb3d
- Agarwal argues ads are so efficient because they allow fine-grained differential pricing (charging each user close to their value), where the top few percent of queries or users fund the rest. (§ Shapley Values: “the top few percent of search queries subsidize all of the rest”) ^clm-2760185f5abea2639e1c
- Agarwal says exact Shapley values cost more to compute than the payment they decide, so Parallel spent a year to a year and a half building a model that estimates them, trained on costly simulations. (§ Parallel AI: “it’s like more expensive to compute how much to pay a content owner than to just pay them”) ^clm-6f864a396a60e9a69ff2
- Index by Parallel gives each site four scores: Impressions, Citations, Value, and Uniqueness; Uniqueness is where the Shapley math rewards content that others do not also supply. (§ Index: “The Index has four scores: Impressions, Citations, Value, and Uniqueness”) ^clm-9226c02d87ef22445018
- Agarwal says Parallel's early data shows unique facts win, with local news and PR Newswire getting outsized value, and plans to publish findings over time. (§ Index: “we see pop from the data is local news ends up being more valuable”) ^clm-ac2fb07c088e957ec64f
- Thompson reports that Stratechery scored highest on Value in the Index but dropped sharply on Uniqueness, while nyc.gov shot up on Uniqueness. (§ Index: “Stratechery did very good on Valuable, that was my highest score, but I plummeted on Unique”) ^clm-9733f7eddc34009b3404
- Agarwal says content that gives agents a recipe, a plan for how to tackle a kind of problem, is also cited and rewarded, not just raw facts. (§ Index: “giving a recipe to an agent to tell it how it should go about doing some work”) ^clm-c5f66ebcb55b87d91ec4
- Agarwal says Parallel's product has been in market for about nine months, selling a search index plus search agents on top, used by customers like Notion and Harvey. (§ Content Marketplaces: “in the last sort of 9 months since we’ve had the product out in the market”) ^clm-1aa8af7805969c39e2de
- Agarwal says Bing shut its public search API a couple of years ago and Google offers no search API at scale, leaving OpenAI's bundled search tool as a common starting point. (§ Content Marketplaces: “Bing used to have a public API, which they shut down a couple of years ago”) ^clm-fc22ab9a5dbfdb83e21e
- Agarwal argues much ad spend now counted as consumer is really B2B, such as a startup buying Google ads to reach business buyers, and in an agent world that spend will flow through agents doing high-value work. (§ Content Marketplaces: “we’ve been miscategorizing a bunch of ad spend as consumer that’s actually B2B in this agentic future”) ^clm-06797853c0a1226ab48b
- All of Parallel's APIs are pay per use; a customer can set a budget like $0.10 for a query and pay more to continue, and the API flags low confidence so an agent can decide to spend more. (§ Content Marketplaces: “All of our APIs are paid by the use”) ^clm-95fe5f70ee9cac3ee600
- Agarwal argues the open web will not stay open if its business model fails, and that paying content owners is a business argument, not a moral one. (§ Content Supply: “We’re not building this compensation thing out of like the fondness of our hearts or making a moral argument”) ^clm-0c38de769e038d04b50a
- Parallel's first paid content partners include PR Newswire, PitchBook, Tracxn, Fortune, and The Atlantic, plus independent writers like Azeem Azhar and Alex Heath. (§ Content Supply: “Today we announced our first set of partners to whom we’re starting to pay”) ^clm-bcb3ff738b03e5a8d745
- Agarwal says payouts come from a shared pool, like Spotify, that grows with how much agents use the web, and split by Shapley value. (§ Content Supply: “the pool is calculated based on how much agents use the web”) ^clm-e60abd820e9bf9f172d0
- Prediction: Agarwal predicts that if models and intelligence keep getting cheaper, data becomes more valuable as the complement, so a larger share of spend may go to content over time. (§ Content Supply: “if the complement of data is commoditized, data becomes more valuable”) ^clm-daafe3ac30f13cb3ac12
- Agarwal says paywalled or login content can only be reached through an Index content partnership, and open content is crawled only if the owner allows it. (§ Competitors and Partners: “the only way we can access them is via a content partnership via the Index by Parallel system”) ^clm-2b5508db4182092724d3
- Agarwal says Parallel complements model makers like OpenAI and Anthropic rather than competing with them, and is usually bought alongside their models. (§ Competitors and Partners: “we are building what is a complement to the best model”) ^clm-e33601b53b917c709c93
- Agarwal says Cloudflare's Matthew Prince has the same diagnosis that the open web could die, and Cloudflare can create scarcity while Parallel knows what content is worth from the demand side. (§ Competitors and Partners: “they’re uniquely positioned to create that scarcity”) ^clm-03b15684007ed44c0db4
- Agarwal says the 1000x agent usage forecast from two and a half years ago now looks too low, and demand is growing very fast. (§ Competitors and Partners: “we felt like we were crazy — today, I feel like we undershot”) ^clm-d53aa5589f963ee3a8a3
- Agarwal says Parallel's marketplace covers only data agents use at inference time (when answering), not training data, because no one yet knows how to attribute training data. (§ Competitors and Partners: “We focus exclusively on data used by agents at inference time and not for training or pre-training”) ^clm-5618f36d93f27c14caef
- Prediction: Agarwal predicts that if demand keeps growing as forecast, within two years people will change behavior and create content aimed at gaps agents need filled. (§ Competitors and Partners: “you will see people change behavior, create pay-walled or non-pay-walled content”) ^clm-171d726d35fdf0ed75f7
- Agarwal says agents so far do not care about the quality of writing, and Thompson argues agents ignore the storytelling that makes content work for humans. (§ Competitors and Partners: “so far I haven’t seen agents really care about quality of writing”) ^clm-ed8119e57dd3d93b3c4a

## Entities

[[Anthropic|Anthropic]], Cloudflare, [[Elon-Musk|Elon Musk]], [[Google|Google]], Harvey, [[Jack-Dorsey|Jack Dorsey]], [[Microsoft|Microsoft]], Notion, [[OpenAI|OpenAI]], [[PR-Newswire|PR Newswire]], [[Parag-Agrawal|Parag Agrawal]], [[Parallel|Parallel]], PitchBook, [[Twitter|Twitter]]

## Concepts

[[AI-Agents|AI Agents]], [[AI-Compute-Demand|AI Compute Demand vs Supply]], The Agentic Web, [[Conservation-of-Attractive-Profits|Conservation of Attractive Profits]], Shapley Values
