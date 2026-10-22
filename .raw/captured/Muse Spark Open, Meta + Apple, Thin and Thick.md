---
title: "Muse Spark Open, Meta + Apple, Thin and Thick"
source: "https://stratechery.com/2026/muse-spark-open-meta-apple-thin-and-thick/"
author:
published: 2026-10-20
created: 2026-10-21
description: "Meta has a new open source model, and to everyone’s surprise, they are are partnering with Apple to make sure you can run it locally."
tags:
  - "clippings"
---
**Listen to this post:**

Good morning,

On [last week’s episode of Sharp Tech](https://sharptech.fm/member/episode/apple-enters-the-uncanny-valley-the-space-x-play-for-cellular-q-a-on-the-ringer-smartphones-ai-parenting), Andrew and I discussed Apple’s plans for the home, SpaceX’s plans for cellular, and how AI can make for better parenting.

On to the Update:

### Muse Spark Open

From the [Wall Street Journal](https://www.wsj.com/tech/ai/meta-and-apple-longtime-foes-team-up-to-put-open-weight-ai-on-macs-a28fde11):

> Mark Zuckerberg has battled Apple ever since the early days of the iPhone. Now artificial intelligence has brought the two fierce rivals together. Meta Platforms said Thursday that it was releasing a new open-weight AI model and collaborating with Apple to run it locally on the company’s high-end Mac computers. The tech giants’ partnership gives developers another American-made AI option to power research projects, app development, video production and more…As part of the collaboration, Apple updated its MLX software toolkit to enable Meta’s model to run well on Macs.
> 
> Open-weight models have their core components released to the public, meaning anyone can download them. Many popular, low-cost Chinese models are open-weight, including Alibaba’s Qwen, DeepSeek and Moonshot’s Kimi K3. Other American open-weight offerings include Inkling from Thinking Machines and Nemotron from Nvidia, which released three new models on Thursday.
> 
> Meta said its new model, called Muse Spark Open, was built for coding and agentic work but acknowledged that Chinese open models are still superior for software development and some other tasks. It is the second open-weight model Meta has released since the company overhauled its AI efforts last year.

Muse Spark Open is an important release; it also, like past Meta open weight model releases, comes with more restrictions than your typical open source license:

- Products built with the model must display “Built with Muse Spark Open”
- There is an acceptable usage policy prohibiting certain behaviors
- Companies offering the model as a service must enter into a commercial agreement with Meta if their total annual revenue exceeds $20 million.

That’s the first difference from at least some Chinese models: [DeepSeek-V4.1-Flash](https://huggingface.co/deepseek-ai/DeepSeek-V4.1-Flash-1017), for example, has an MIT License, while [Qwen’s smaller models](https://huggingface.co/Qwen/Qwen3.8-27B) have an Apache license; both are effectively free to use as you wish. Other models, however, like [Kimi K3](https://huggingface.co/moonshotai/Kimi-K3) or [the largest Qwen models](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B/blob/main/LICENSE), have similar restrictions to Meta.

The second difference from Chinese models is that Muse Spark Open is not as good, but that’s to be expected. First, this is based on a six month old model that was a few releases behind when it came out in April. Second, however, I continue to think it is important to acknowledge the role of distillation; I wrote in [Who’s Afraid of Chinese Models](https://stratechery.com/2026/whos-afraid-of-chinese-models/):

> I think it is mistaken to attribute all of the success of Chinese labs to distillation, but it’s just as much of a mistake to pretend like distillation doesn’t give Chinese labs a big advantage…Because U.S. open weight model makers must follow the frontier labs’ terms of service, they (1) are worse than Chinese alternatives and (2) end up distilling the distillation, just with a detour through Chinese labs. Wouldn’t it be better if western open weight model makers could go to the source?

I don’t know if Meta distills Chinese models, but I’m pretty confident they don’t distill frontier models, and that unfortunately means they are at a disadvantage to Chinese models, at least in the short term. The long term, however, could be more optimistic: Meta continues to invest heavily in research — both in terms of humans and especially in infrastructure — and the rate of progress is impressive. Muse Spark Open comes on the heels of the closed release of Muse Wonder, which presumably will be an open source model in a few months; if these models continue to be built from scratch they have a chance to be the most compelling open weights option on the merits.

More than that, though, they are American; there are obvious concerns in terms of building dependencies on Chinese models for Western enterprises and government. Just this week, in fact, the [Department of Homeland Security mandated that federal civilian agencies rid themselves of DeepSeek models](https://www.wsj.com/tech/ai/dhs-orders-deepseek-technology-removed-from-federal-civilian-it-systems-060b6d3d); I wrote in that Article I referenced above:

> There are and will be models eminently capable of mounting cybersecurity attacks on existing infrastructure, and those models will be — already are — widely available. The best defense — the only viable defense, in fact — will be to make sure defenders have access to the best models as well. Right now defenders are effectively banned from using Fable or Sol for cybersecurity because of Trump administration directives; that means the best alternative is using models from a country which has been trying to weaken our cyber defenses for years. This is insane!

[Meta has announced it wants to sell to enterprise](https://stratechery.com/2026/one-more-note-on-agents-meta-connect-meta-enterprise-platform/), so it wasn’t certain it would continue to open source models; this isn’t incompatible with that strategy, however: it’s plausible to imagine a go-to-market approach predicated on selling to companies that start out with Muse models because they are free to get started and then want to access them as a service when their usage takes off. We’ll see if that strategy continues to make sense if Meta ever does truly make it to the frontier — I hope so.

### Meta + Apple

What is especially interesting to me, for multiple reasons, is this partnership with Apple. [I’ve long made the case](https://stratechery.com/2020/apple-and-facebook/) that Apple and Meta are structural partners: they may dislike each other, but they can’t help but make each other’s business better. In this case, however, perhaps because of the replacement of Tim Cook with John Ternus as Apple CEO, there is an actual thawing of the relationship.

I know this because there I was on Apple’s campus last Wednesday, walking into an Apple conference room, where I was greeted by some Apple people I didn’t know, along with Meta Head of Compute and Stratechery Interview guest [Daniel Gross](https://www.axios.com/2026/10/15/apple-and-meta-bury-the-hatchet-for-ai)! It was, needless to say, a pleasant surprise on multiple counts. I don’t want to overstate the degree of cooperation here: from what I understand Apple made specific MLX changes to benefit Meta, although those changes will be broadly available, and Meta made some changes to how the model worked to optimize the Mac Studio’s architecture. Still, the symbolism of that room was notable.

To that end, the real stars of the show were sitting at my table: two Macs Studio with 512GB of unified memory linked together with four Thunderbolt 5 cables; an Apple engineer proceeded to do a number of demonstrations on the devices, including working on a mobile app (I originally said “writing code”, but we’re well past that point with these models), and producing a clip compilation from a huge amount of footage from a TV set.

I found the second demo more compelling than I expected: video files are enormous, and upload bandwidth, particularly on location, is very dodgy; even if a production crew wanted to use a cloud model it’s not clear that would be viable for something they wanted same day. In that scenario a cart with a couple of Macs Studio — that, critically, plug into a wall — is providing functionality to a television crew that simply wouldn’t exist otherwise.

It’s the coding possibilities, however, that I found particularly compelling. The Macs Studio were definitely slower; tokens, however, were effectively free, and that made me want to see a different demo entirely. Consider how humans code: usually you implement something once, because coding is very costly in terms of time and effort; if it works you stick with it. That’s basically how AI coding works today as well, including in the demo I saw: the Apple presenter typed in a prompt to alter an app he was working on in Xcode, and Muse Spark Open “one-shotted” it.

This is very, to use CPU terminology, single-threaded in its approach. CPUs, however, long ago moved beyond strictly serial execution: [branch prediction](https://stratechery.com/2018/meltdown-spectre-and-the-state-of-technology/) lets them speculatively execute instructions before knowing whether those instructions will actually be needed. If the prediction is correct, the work is already done; if it’s wrong, the work is discarded and the CPU starts down the correct path. Recalculating the correct path is considered “expensive”, but that’s relative: it’s time that would have been spent absent the prediction, which is costless.

What if a coding harness were to operate the same way? Imagine if the coding harness built multiple variations of a feature overnight, with various permutations based on each different path; then when you reviewed the work in the morning, you could not simply make a binary yes/no decision, but rather choose from a list of already-built options, each of which has follow-on features based on your choice already built. It’s basically branch prediction, but at a massively higher level of abstraction.

This approach would be cost prohibitive if you were paying for usage; if inference is running locally, however, then you have effectively unlimited tokens, which means throwing away unused paths is costless. You are, of course, paying for the electricity the Macs Studio use, but that cost is so much less than traditional GPUs, and you don’t need to buy dedicated air conditioners either! Meanwhile, you have an entirely new way of working that is something different and more compelling than human-style coding done at superhuman speed.

### Thin and Thick

Earlier this year I declared that [Thin Is In](https://stratechery.com/2026/thin-is-in/):

> This combination of factors will only accentuate the dominance of the thin client paradigm:
> 
> - First, if compute isn’t yet good enough, then workloads will flow to wherever compute is the best, which is going to be in large data centers.
> - Second, if larger models and more context makes for better results, then workloads will flow to wherever there is the most memory available.
> - Third, the expense of furnishing this level of compute means that it will be far more economical to share the cost of that compute amongst millions of users; guaranteeing high utilization and maximizing leverage on your up-front costs.
> 
> Yes, you can run large language models locally, but you are limited in the size of the model, the size of the context window, and speed. Meanwhile, the superior models with superior context windows and faster speeds don’t require a trip to the computer lab; just connect to the Internet from anywhere. Note that this reality applies even to incredible new local tools like OpenClaw: OpenClaw is an orchestration layer that runs locally, but the actual AI inference is, by default and in practice for most users, done by models in the cloud.
> 
> To put it another way, to be competitive, local inference would need some combination of smaller-yet-sufficiently-capable models, a breakthrough in context management, and critically, lots and lots of memory. It’s that last one that might be the biggest problem of all.

The Mac Studio is a bit of a breakthrough in that it can run a model this capable this well; that noted, all three of my points hold:

- Muse Spark Open is not as good as frontier models (including Meta’s), and the Macs Studio are not nearly as capable as what is available in the cloud.
- Therefore, all things being equal, workloads should run in the cloud.
- Given that a reasonably equipped 512GB Mac Studio is probably going to be approaching $20,000 or so, even API costs — much less subscription prices — are likely going to be much more attractive for most people.

Moreover, two Macs Studio acting as your own personal AI server is still a thin architecture: the Apple presenter was actually working on a MacBook Pro, using the Macs Studio headlessly; the thickness just happened to be in the room with us.

Setting aside that last point, however, realizing the potential of this configuration does depend on (1) local models becoming “good enough” and (2) unlocking new ways of working that start with the assumption that tokens are free.

Even there, however, you can envision a world where compute is no longer scarce, and very cheap models in the cloud are also good enough; it’s hard even then to see local inference penciling out economically. That’s why the true case for this setup may ultimately depend not on free as in beer but free as in speech: what makes me truly excited about this setup is the certainty of knowing I can truly do whatever I want. That’s not nothing, and it’s very much in [Apple’s ethos in particular](https://stratechery.com/2018/techs-two-philosophies/).

---

This Update will be available as a podcast later today. To receive it in your podcast player, [visit Stratechery](https://stratechery.passport.online/member).

The Stratechery Update is intended for a single recipient, but occasional forwarding is totally fine! If you would like to order multiple subscriptions for your team with a group discount (minimum 5), please contact me directly.

Thanks for being a subscriber, and have a great day!