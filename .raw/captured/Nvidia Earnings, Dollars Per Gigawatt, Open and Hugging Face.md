---
title: "Nvidia Earnings, Dollars Per Gigawatt, Open and Hugging Face"
source: "https://stratechery.com/2026/nvidia-earnings-dollars-per-gigawatt-open-and-hugging-face/"
author:
published: 2026-09-01
created: 2026-09-09
description: "Nvidia’s earnings were remarking and boring — two sides of the same coin. Everything the company does is about avoiding a consolidated world."
tags:
  - "clippings"
---
**Listen to this post:**

Good morning,

Over on [Asianometry](https://asianometry.passport.online/member/episode/the-little-ceiling-robots-inside-a-semiconductor-fab), Jon has a delightful video about [The Little Ceiling Robots Inside a Semiconductor Fab](https://asianometry.passport.online/member/episode/the-little-ceiling-robots-inside-a-semiconductor-fab).

On to the Update:

### Nvidia Earnings

From [Bloomberg](https://www.bloomberg.com/news/articles/2026-08-26/nvidia-estimate-topping-forecast-fails-to-wow-investors):

> Nvidia Corp., the chipmaker at the heart of the artificial intelligence boom, projected sales growth of 70% for the next fiscal year, sending its shares on their biggest one-day rally since April 2025. The forecast far outstripped the average analyst estimate of 45%, according to data compiled by Bloomberg. And Nvidia would be growing even faster if it had access to more supplies, Chief Financial Officer Colette Kress said during a post-earnings conference call.
> 
> “Incredibly, we are seeing demand acceleration even at our scale,” she said. “Customers’ forecasts point to our growth doubling next year.” Nvidia shares rose 8.7% to $227.98 in New York on Thursday, adding about $442 billion in market value. That left the stock up 22% for 2026.
> 
> The upbeat outlook offered relief to investors concerned about a bubble in the AI economy. Nvidia, the world’s most valuable company, is the leading provider of AI accelerators, a key component for training and running artificial intelligence models. That status has turned its quarterly earnings into a barometer on the state of the wider industry.

Every time I think I’m insufficiently bullish, by virtue of being exposed to tech exuberance, I read summaries like this and remember that I am certainly very far down the curve of believing in AI. Way back in February 2024, [I wrote in response to Nvidia’s earnings](https://stratechery.com/2024/nvidia-earnings-inference-and-meta/):

> Here’s the key point: if Nvidia demand exceeds supply then the company’s sales are, in some respect, controlled by Nvidia’s suppliers, from TSMC on down. Now that’s not completely true, because Nvidia can raise its prices, and it appears they did just that: the company achieved its highest gross margins ever, and forecasted the same thing this quarter. That, though, only accentuates the fact that the company is supply-constrained in a world of astronomical demand.

Here we are two-and-a-half years later and Nvidia is without question still limited by supply. That is the subtext of the company providing a forecast for not just the next quarter but for its entire next fiscal year. Here was CEO Jensen Huang on [the earnings call](https://seekingalpha.com/article/4940563-nvidia-corporation-nvda-q2-2027-earnings-call-transcript):

> It is also the case that you can no longer procure technology per se and stand up this infrastructure. You’ve got to go secure the land, power and shell, which oftentimes is a couple 2, 3 years out. All of the rest of the supply chain necessary to align the construction, the power, the cooling, all of the labor that’s necessary. AI infrastructure is creating so many jobs all over the United States and all around the world. It just takes a lot more planning. And so we’re involved in securing infrastructure now further down the pipeline. Just as a long time ago, people asked me why is it that we’re working with memory suppliers when we’re a chip company. And today, people understand it’s really quite genius that we were working on our supply chain so far upstream. We work with power generator companies, we work with land, power and shell companies all around the world. And that helps prepare all of this computing that’s going to be built that will ultimately deploy for our ecosystem and our customers. And so, we just have a lot greater visibility now upstream and downstream.
> 
> It is the case that we’ve never forecasted or never guided to a year in advance. And even though our demand is much greater than 70%, our supply allows us to confidently deliver 70%. And we’re going to continue to work with our supply chain to increase on that. But what we wanted to do is to be consistent with everybody, from our customers, our shareholders, our supply chain, everybody sees the same view. And the reason why that’s important is because everybody is putting a lot of resources at play. And so we wanted to make sure that everybody has the same set of information. And we’ve got a huge year coming up next year, and it’s going to be pretty extraordinary.

I’ve made this analogy before, so bear with me, but Nvidia right now continues to be like Apple in the early years of the iPhone: for years forecasting was easy and reliable, because the company’s revenue was a function of how many phones they could make and how many carriers they supported; we didn’t truly know what iPhone demand was until the iPhone 6S generation, when supply was sufficient and every carrier had the iPhone.

We’re seeing the same story here: Nvidia’s earnings really ought to be quite boring, because the top-line revenue number is a function of how much supply the company will have in terms of components; we won’t know what demand truly is until supply is abundant. And, to that end, I think that the company was trying to send that exact message with this longer-range forecast: not only does Nvidia have better visibility and access to its supply chain than anyone else, it also is not even close to seeing demand being met.

This is, to be clear, pretty extraordinary. Yes, the iPhone run was longer, but it wasn’t at these revenue levels. Nvidia grew 100% and is forecasting growth of “only” 70%, but that number is unquestionably a function of supply not demand — and we’re coming up on the four-year anniversary of ChatGPT. There is no sign any of this is slowing down, and when you consider the explosion in capability that has happened just this year, it’s fair to assume that Nvidia would still be accelerating if it could actually meet demand.

### Dollars Per Gigawatt

Nvidia tends to approach these calls with a specific message management wants to land, and this call was all about the company capturing an ever greater percentage of data center TAM, which, combined with the increased value of AI, meant that Nvidia’s growth should be understood as a function of $/GW. Secondly, this increase in TAM was most pronounced outside of the hyperscalers — the sub-theme of this call was that Nvidia’s market opportunity extended beyond Big Tech.

Here’s CFO Colette Kress on the first point:

> Our full-stack AI factory platform…is expanding our share of the data center TAM. Since Hopper, our revenue opportunity has grown from roughly $18 billion per gigawatt to $25 billion with Blackwell, to $40 billion with Vera Rubin, which now spans Vera CPU, Rubin GPU, NVLink, InfiniBand or Ethernet and Groq LPU announced earlier this week. Our ability to extreme co-design across GPU, CPU, NVLink scale-up networking, scale-out networking, systems, algorithms and software enables us to deliver X factor performance gain every generation. Vera Rubin exemplifies this, delivering 30x higher throughput per megawatt and 35x lower token costs relative to Grace Blackwell Ultra.

Huang made the point — repeatedly — that this level of integration was underpinning the entire non-hyperscaler market:

> The part that people don’t see about our growth because we’re practically singular because of the nature of how we deliver products. I mean we’re the only company in the world that creates and builds, offers an entire AI factory platform, a full-stack system. Customers can still mix and match. However, most companies just don’t have the skills to do that or desire to do that. And so there’s an entire part of the market that we experienced growth. There is sovereign AI, there are regional AIs, there are neoclouds, there are AI start-ups, there are enterprises, which represents about half of our business, and that’s growing 100% a year. That part of the world’s computing is likely to be larger over time than even what we’re currently experiencing in the cloud. And so I think the demand that we see is driven by all of those factors. It is also the case that you can no longer procure technology per se and stand up this infrastructure. You’ve got to go secure the land, power and shell, which oftentimes is a couple 2, 3 years out. All of the rest of the supply chain necessary to align the construction, the power, the cooling, all of the labor that’s necessary.

The last sentence is a compelling argument: when you have so many other problems to solve, worrying about Nvidia’s margins is often at the bottom of the list. To put it another way, when there are many difficult pieces, the integrated piece that solves multiple problems at once is particularly valuable.

Unless, of course, you have the sort of scale that makes it possible and profitable to solve every problem you have — including Nvidia’s margins. That’s the hyperscalers. Or, in the case of the frontier labs, have so much demand and such high costs that you both have to figure out a way to capture more margin and have the potential payoff to justify it. To that end, I thought Huang’s answer about [OpenAI’s new chip](https://stratechery.com/2026/apple-updates-mini-and-studio-ai-computers-openai-jalapeno/) wasn’t particularly convincing:

> Well, we’re building something very different. Whereas many of these XPUs are inference-specific chips for one cloud or one service, Nvidia is a platform, an entire AI factory platform that spans the entire AI life cycle that you can use in any cloud, it’s in every cloud. You can run anywhere. We’ll help you set it up anywhere. And so we built something very different. All of the AI services at some point are going to want to go around the world. And those data centers won’t necessarily be just built by them. And also, I think they’re going to run on NVIDIA all around the world. And of course, I think our technology, I have 100% confidence that our technology will continue to be extraordinary for them, and that the economics of using our technology, whether it’s from data processing to training to post training to agentic processing, our technology is going to be extraordinary for them. They’re going to use it. And so I’m very confident that they’re going to be customers and partners of ours for a very long time.

That’s about five different answers, none of them particularly compelling in a potential world where the frontier labs [just win everything](https://stratechery.com/2026/whos-afraid-of-chinese-models/); perhaps that is why Huang followed up his answer salad by reminding investors that Nvidia holds huge stakes in both companies. And then he went back to talking about $/GW.

### Open and Hugging Face

This was Huang’s answer about open source models (i.e. open weights):

> The world will need both closed models and open models. And both closed models and open models are skyrocketing in use. Near most, I would say, nearly all open models run on Nvidia, and the reason for that is because Nvidia’s footprint around the world is the highest, and our architecture is the most fungible. It’s everywhere. It’s in PCs and edge devices like DGX Spark, which is doing great, all the way to robots and workstations and your on-prem data centers. Open models are doing incredibly well. Closed models, we know are doing incredibly well. The frontier labs, their scale, their sales are skyrocketing, their margins are fantastic. They’re generating profitable tokens. They are only limited by the amount of compute. That is equally true for open models. And our position in open models is very good because the CUDA ecosystem is literally everywhere.

Open weights are the model equivalent to Nvidia’s ACIE segment. As long as the world is fragmented Nvidia wins; the only way its margins come under pressure is if there are a limited number of buyers who have the means to take only part of Nvidia’s stack or replace them completely. In a world of choices, however, the most fungible architecture with the deepest developer pool has a huge advantage, and Nvidia continues to pull out all of the stops, particularly from a capital perspective, to make that happen.

What hasn’t happened officially — although it was reported as such by [The Information](https://www.theinformation.com/articles/nvidia-agrees-buy-open-source-model-repository-hugging-face-12-9-billion) — is Nvidia buying Hugging Face, the open model hosting service. Again, this deal hasn’t been announced yet, but I think a lot of the speculation as to why Nvidia might do this is over-complicating things. For example, from that report:

> Nvidia, by buying Hugging Face, would in effect be resuscitating its AI cloud business, a business it backed away from a year ago. The business, DGX Cloud, had put Nvidia in quasi-competition with Amazon Web Services. Nvidia had committed to spend $13 billion to rent back its own AI chips from bigger cloud providers that had purchased them, including AWS. Nvidia has then turned around and rented out some of those chips to companies such as Amgen and ServiceNow that develop their own AI applications. Nvidia believed the cloud business could one day help it generate $150 billion in revenue.
> 
> Hugging Face could also serve as a contingency plan. Nvidia said during earnings that it had committed to $36 billion in cloud services contracts as part of credit support agreements with its customers. If market conditions shift and customers aren’t able to lease that capacity out to third parties, Nvidia would end up responsible for some of that compute. And if Nvidia finds itself with more compute than its own engineers can use, it could use the capacity to power AI for Hugging Face customers while expanding that business.

This is overthinking things. Hugging Face is a critical Schelling point for open source models, much like GitHub was for open source software a decade ago. And, just like it made sense for Microsoft to acquire GitHub even without an obvious financial model that would justify the price — simply because Microsoft cared about developers and wanted additional in-roads to developers not necessarily on Microsoft platforms — it makes all kinds of sense for Nvidia to acquire Hugging Face to ensure that an essential piece of the open source ecosystem thrives. Nvidia doesn’t need to make money from Hugging Face, or mandate that Hugging Face-hosted models use Nvidia chips or anything like that; simply ensuring that open weights have a meaningful future structurally ensures Nvidia’s long-term margin profile.

Other than that, it’s funny how the seminal public AI company’s results are boring and/or predictable. That, however, speaks to how remarkable this moment continues to be: we won’t know the answer to many of these questions until supply exceeds demand, and that moment seems further out than ever.

---

This Update is also available as a podcast. To receive it in your podcast player, [visit Stratechery](https://stratechery.passport.online/member).

The Stratechery Update is intended for a single recipient, but occasional forwarding is totally fine! If you would like to order multiple subscriptions for your team with a group discount (minimum 5), please contact me directly.

Thanks for being a subscriber, and have a great day!