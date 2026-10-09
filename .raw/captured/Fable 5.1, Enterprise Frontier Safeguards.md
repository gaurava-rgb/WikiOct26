---
title: "Fable 5.1, Enterprise Frontier Safeguards"
source: "https://stratechery.com/2026/fable-5-1-enterprise-frontier-safeguards/"
author:
published: 2026-09-02
created: 2026-09-09
description: "Fable 5.1 is out, and the hated Fable data retention policy is not just being altered, but entirely removed in the meantime. Plus, why increased caching is a win-win."
tags:
  - "clippings"
---
**Listen to this post:**

Good morning,

Two scheduling notes: first, summer is over and Stratechery Interviews are back. However, this week’s Stratechery Interview will not publish tomorrow, but on Friday, so look forward to that (relatedly, Sharp Tech will publish on Thursday, not Friday). Second, next Monday is Labor Day; there will be no Update.

On to the Update:

### Fable 5.1

Anthropic announced Mythos 5.1 and released Fable 5.1 yesterday; as Anthropic noted in [their introductory blog post](https://www.anthropic.com/claude-fable-and-mythos-5-1):

> Claude Fable 5.1 and Claude Mythos 5.1 are the same model, but with different levels of safeguards. Fable 5.1 is generally available, while Mythos 5.1 is available only through our trusted access programs; its safeguards are specifically designed to support work in cybersecurity and the life sciences.

I obviously don’t have access to Mythos, but it’s interesting that Anthropic felt it was necessary to make clear in the first sentence that Fable is the same model; it is, given its general availability, the more pertinent one from a business perspective. From [Bloomberg](https://www.bloomberg.com/news/articles/2026-09-01/anthropic-says-new-fable-5-1-ai-model-is-cheaper-better-at-coding):

> Anthropic PBC is releasing a new version of its powerful Fable artificial intelligence model that it says is better at coding and science tasks, as well as more economical — all changes it says are in response to customer feedback. The company said Fable 5.1, which it plans to release on Tuesday, is more skilled at carrying out lengthy, complicated computer programming tasks, such as software projects or code reviews that require it to work across all the code for an application. The new version is also better at helping with scientific work like coming up with experiment designs, simulating what could happen during an experiment and reading information in dense diagrams and tables, Anthropic said.
> 
> Companies are increasingly trying to justify and rein in the costs for AI usage at a time when open-weight, lower cost models from China are rapidly improving. These trends are applying pressure to US-based model makers like Anthropic. Anthropic will charge enterprise users the same price per token — a unit of data processed by AI models — for Fable 5.1 as it has for Fable 5, but is lowering the price it charges users when the AI model resurfaces information it had previously processed. Anthropic said the 75% price reduction it’s offering on this part of the process will lead to a “substantial reduction” in the total cost of running the model. The process can account for half or more of the tokens used to carry out some of the lengthier, more complicated tasks people run on Anthropic’s AI models, said Dianne Penn, who leads product management for research and labs at the company.

Cache is particularly important for agentic workflows, which involve a lot of tool use (i.e. actual definitions and schemas which have to be loaded into the context window and which is the same across not just a single user but all users). Cache is, particularly relative to actual generation, much closer to free (the entire Internet is, in many respects, just a massive caching layer; to put it another way, cache is what undergirds zero marginal costs). Therefore, it makes total sense that this is an easy vector for Anthropic to credibly promise lower prices: develop a better cache layer, charge less for tokens from that layer (which is dramatically cheaper), and the price-per-task is lower even if the price-per-generated-token is the same.

Anthropic said about pricing in their blog post:

> Fable 5.1 will cost an estimated 25% less than Fable 5 for typical workloads, wherever usage is billed by token. This is because we’re reducing our pricing on cache reads (where the model reads inputs that have already been processed and stored). For highly agentic work, the savings will often be much larger—up to approximately 45%.

The interesting phrase there is “wherever usage is billed by token”; the implication is that this price cut does not apply to subscriptions, which makes sense: the entire premise of subscriptions is that you are *not* paying per token. What that means for Anthropic, however, is that any savings they can achieve increase their margins on subscriptions. To put it another way, enterprise customers care about the price they pay per token because it impacts how much they pay Anthropic; Anthropic cares about the price it costs to serve per token because it impacts how much it costs to serve subscribers. In this case, something like improved cache usage is a win on both sides of the business.

### Enterprise Frontier Safeguards

From [CNBC](https://www.cnbc.com/2026/09/01/anthropic-data-retention.html):

> Anthropic on Tuesday announced it will change a controversial data retention policy for its business customers after “a lot of feedback,” and it said it plans to implement a new solution called Enterprise Frontier Safeguards instead. The company introduced its existing data retention policy in June alongside the launch of Claude Fable 5 and Mythos 5, two of the company’s most advanced artificial intelligence models. Anthropic said at the time that it would require 30-day retention for all traffic on those models to help defend against misuse and “complex and novel” cyberattacks. Anthropic pledged not to use that data for any “non-safety-related purpose,” including model training, but many of its enterprise users expressed concern.
> 
> Kate Jensen, head of Americas at Anthropic, told CNBC that the company spent hundreds of hours working with customers to develop another solution. With the launch of Enterprise Frontier Safeguards, Anthropic said businesses will be able to control how their data is reviewed, stored and managed, and they will also be able to carry out automated safety monitoring where no Anthropic human review is required. The company said it will not charge for Enterprise Frontier Safeguards, and that the controls will work whether users access Anthropic’s technology directly or through a cloud provider.

There was something I found very humorous about this news. First, because I’m a business nerd, I found it to be the most interesting revelation yesterday. Second, while the Fable release was at the top of Techmeme all day, this item was buried halfway down the page. Third, the [Fable item](https://www.techmeme.com/260901/p34#a260901p34) had a ton of posts on X linked; the [Enterprise Frontier Safeguards item](https://www.techmeme.com/260901/p36#a260901p36) had a bunch of LinkedIn posts. Alas, the implications of this paragraph are not great for me, but I must follow my heart.

Anyhow, this item was very interesting to me, and closes the loop on what I thought was one of the most interesting aspects of the original Fable release. I wrote when [Anthropic changed its data retention policy terms for Fable](https://stratechery.com/2026/fable-5-anthropic-alignment-ai-tiers/):

> It’s pretty significant, I think, that Anthropic is declaring that not retaining data is no longer an option, at least if you want access to their best models. Yes, today, that retention is for safety purposes only, and not for training; it’s plausible, however, that Anthropic’s lead becomes so significant that they quietly announce that they are going to train on that data as well, and companies will feel they have no choice but to go along. That additional training data, of course, will only further increase Anthropic’s lead, and all of this will be justified because Anthropic has already clearly decided they are the only ones who can be trusted to be in charge.

Then, last month, [this report from Ramp](https://econlab.substack.com/p/ai-index-august-2026) made waves asking “Why aren’t businesses using Fable 5?”:

> Last month, Anthropic released the best AI model to ever hit the market, Fable 5, and we now have the first public data to share business uptake of the model so good its release was briefly blocked by the U.S. government: one month in, businesses aren’t using it that much. Over the last month, Fable 5 has made up only 6% of tokens businesses purchased from Anthropic, and despite being their most expensive model by far, 11.4% of dollars spent on Anthropic models. For comparison, OpenAI’s flagship model, GPT-5.6 Sol, comprises 25% of OpenAI tokens and 23% of spend. In fact, Fable 5 is less popular with businesses than GPT-5.6 Sol overall. In July, Fable 5 generated approximately 75% as much model-attributed spend as GPT-5.6 Sol.
> 
> So why does this make me wary of the AI trade? Fable 5 is the most performant model on the market. It’s also the most expensive, at roughly $10 per 1M tokens, twice as expensive as the still highly performant GPT-5.6 Sol. So with Fable 5, we’ve found a new upper bound for how much businesses are willing to spend on AI. Here, more performance is not worth the price tag. To encourage business adoption of the latest models, the labs will need to prove performance beyond what even Fable 5 is able to achieve and simultaneously ensure that competitors aren’t able to come reasonably close. That seems increasingly out of reach, especially as open source models catch up to being only a few months behind.

I do think that price was probably the biggest reason for Fable’s relatively low penetration; I accidentally blew through my subscription limits a few weeks ago, added some credits, and was shocked at how much I was paying to finish the project I was working on. If you’re using Fable you need to be really sure it’s the right model for the job, or the price bites quickly.

At the same time, I don’t think the data retention policy change helped. Anything but a zero data retention policy is, for most large enterprises, simply a no-go. Indeed, arguably the biggest impact of Anthropic’s policy change was putting wind in the sails of companies like Microsoft; that is when Satya Nadella really started to publicly press on the issue of sharing data with the frontier labs, and is a reason why Alex Karp gave [that wild interview](https://stratechery.com/2026/muse-image-grok-4-5-alex-karp-on-cnbc/).

Importantly, the pushback seems to have carried the day. Even if you want to give Anthropic the benefit of the doubt and assume that retaining the ability to analyze data for safety reasons was legitimate, the idea that that data *would be stored by Anthropic* was obviously a non-starter, and I said as much at the time; from [Anthropic’s Safety Superpower](https://stratechery.com/2026/anthropics-safety-superpower/):

> Anthropic upped the ante in a major way with Fable, announcing that they would retain the data for all usage for 30 days, even for their enterprise plans that previously promised zero data retention. The company said they would not train on this data, but they didn’t put in any sort of safeguards to guarantee they wouldn’t do so in the future (like storing the data with a third party). If this policy change (whenever Fable is restored) doesn’t lead to a significant loss of customers, I suspect it’s only a matter of time until they start using the data: it’s simply too valuable to their end goals.

Anthropic might not have lost customers, but [growth did slow](https://stratechery.com/2026/nvidia-backs-openai-data-center-anthropic-news-google-buys-spirit-airlines-data/) and Fable usage was stagnant; thus Enterprise Frontier Safeguards. From the blog post:

> Our new system of Enterprise Frontier Safeguards (EFS) gives customers complete privacy (the same as a zero data retention policy) while still being state-of-the-art at preventing adversarial use. EFS works by storing data in cloud infrastructure controlled entirely by the customer, not Anthropic. It will be made available to enterprise customers in phases, beginning later this fall. Until EFS is available, eligible customers will be able to use Fable 5.1 with zero data retention.

That last sentence is the tell. Apparently the safety concerns aren’t so great that Anthropic can’t revert to a true zero retention policy until the new system is in place; that strongly suggests that my suspicions about where things were trending were correct. And that’s actually good news: competition works, customers can push back, and at the end of the day, the fact that Anthropic needs to make money will be a curb on their worst impulses. For-profit enterprise is the best alignment organizing principle there is.

---

This Update is also available as a podcast. To receive it in your podcast player, [visit Stratechery](https://stratechery.passport.online/member).

The Stratechery Update is intended for a single recipient, but occasional forwarding is totally fine! If you would like to order multiple subscriptions for your team with a group discount (minimum 5), please contact me directly.

Thanks for being a subscriber, and have a great day!