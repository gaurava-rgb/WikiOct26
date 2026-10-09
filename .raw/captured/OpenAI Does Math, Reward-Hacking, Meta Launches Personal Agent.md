---
title: "OpenAI Does Math, Reward-Hacking, Meta Launches Personal Agent"
source: "https://stratechery.com/2026/openai-does-math-reward-hacking-meta-launches-personal-agent/"
author:
published: 2026-09-09
created: 2026-09-09
description: "OpenAI solving one of the most famous math problems is extremely impressive, and of little impact to most people’s lives; Meta’s Muse agent launch has the potential to be the exact oppo…"
tags:
  - "clippings"
---
**Listen to this post:**

Good morning,

Apple’s iPhone event is later today, and I’m going to wait and decide on my publishing plan for Thursday; I have a fun interview in the can, that is a bit out of the normal Stratechery course of things, but if something particularly notable comes up I may cover the event right away. Otherwise I expect we’ll get to it on Monday (and that uncertainty, as I’ve been noting for a few years now, is itself commentary on the iPhone’s position in the ecosystem: it matters because it’s an iPhone, not because it’s new).

On to the Update:

### OpenAI Does Math

From [Scientific American](https://www.scientificamerican.com/article/ai-may-have-just-solved-a-million-dollar-math-problem-the-field-will-never-be-the-same/):

> Today may go down as the biggest day in math in at least two decades, if not far longer. In a development that crystallizes an existential shift in humankind’s oldest intellectual discipline, artificial intelligence has reportedly solved one of the six open “million-dollar” problems in mathematics. The achievement proves that the equations that govern the motion of fluids are fundamentally flawed.
> 
> “This is a Deep Blue–Kasparov moment,” wrote mathematician Tristan Buckmaster, referring to the sea change in thinking about machine intelligence that occurred when a supercomputer beat world champion Garry Kasparov at chess in the 1990s, in a [statement](https://cims.nyu.edu/~tristanb/statement.pdf) released late on Monday. “The community needs to have serious and unhurried discussion about where to go from here.”
> 
> But according to Buckmaster, the proof’s origins may be murkier than they seem. In the same statement, he wrote that he and Levent Alpöge, a mathematician and an Anthropic employee, made significant progress toward the problem last month. But before the pair could publish, Buckmaster alleged in the statement, rumors of their method reached OpenAI, where researchers used the company’s large language model (LLM) to finish the job with a single prompt. The prompt “had been sent in the past few days, after information about our work had reached OpenAI,” Buckmaster alleged. OpenAI did not immediately respond to a request for comment; in a press conference later on Tuesday, the firm [denied](https://www.scientificamerican.com/article/openai-claims-blockbuster-math-breakthrough-amid-swirl-of-controversy/) the allegations.

I’m not going to sit here and pretend that I am a math expert; indeed, the greatest testament to the magnitude of this achievement is that I had actually heard of and was familiar with the [Navier-Stokes problem that OpenAI solved](https://openai.com/index/navier-stokes-solution/).

I’m also, to be honest, not that particularly invested in the controversy surrounding the discovery, specifically [this statement from mathematician Tristan Buckmaster](https://cims.nyu.edu/~tristanb/statement.pdf) insinuating that OpenAI only solved the problem by hearing a rumor that he and Anthropic’s Levent Alpöge were nearing a solution, and more explosively, suggesting that OpenAI may have looked at their chat logs to figure out a direction. I’m actually pretty sympathetic to OpenAI from a PR perspective; Chief Research Officer Mark Chen [wrote on X in response to Alpöge](https://x.com/markchen90/status/2097400166554993041):

![](https://x.com/i/status/2097400166554993041)

Codex and Claude have settings that they say stop your conversation data from being used to train future models, but there are loopholes; for example, from ChatGPT’s [How your data is used to improve model performance](https://help.openai.com/en/articles/5722486-how-your-data-is-used-to-improve-model-performance) page:

> When you use our services for individuals such as ChatGPT and Codex, we may use your content to train our models. You can opt out of training through our privacy portal by clicking on “do not train on my content.” To turn off training for your ChatGPT conversations and Codex tasks, follow the instructions in our Data Controls FAQ. Once you opt out, new conversations will not be used to train our models…
> 
> Even if you have opted out of training, you can still choose to provide feedback to us about your interactions with our products (for instance, by selecting thumbs up or thumbs down on a model response). If you choose to provide feedback, the entire conversation associated with that feedback may be used to train our models.

It’s unclear if Chen or anyone at OpenAI knows if Buckmaster or Alpöge had this setting set; looking that up would itself be a privacy violation, which is how I think we ended up with this seemingly mealy-mouthed non-denial. Or, per this quote, perhaps they hit a thumbs up. In this case, I’m inclined to believe that OpenAI did not explicitly go after Buckmaster and Alpöge’s chats; I also think it’s likely that Buckmaster and Alpöge had this setting turned on; it’s also worth noting, however, that the extremely specialized nature of their work likely means that if any data from their chats were in training sets the models would have paid attention to it.

### Reward-Hacking

It’s the critique from famed mathematician Terence Tao that is the most interesting; from [Mastodon](https://mathstodon.xyz/@tao/117237322698385581):

> Every new advance in mathematics, whether it comes from technique, technology, or infrastructure (such as access to libraries of past literature) reduces the difficulty of solving problems. This is generally a good thing; but it comes at the cost of flattening out the difficulty landscape of a field, to the point where one can no longer discern its geometry to the extent that promising questions can be extracted within the range of applicability of the tool. Often this effect is counteracted by the ability of such a tool to enlarge the radius of the sphere of results one can plausibly reach, creating new boundaries to fruitfully explore.
> 
> However, one notable feature of the current AI era is the absence of any definitive such boundaries. While AI tools have flattened the difficulty landscape now in many areas of the subject, thus destroying the ability to locate promising new problems in that area, there are no clear frontiers that are separating the “AI-feasible” problems from the “AI-hard” problems (which certainly still exist, given that the difficulty level of problems are unbounded, and can even be undecidable). This is in part due to the rapidly changing nature of the technology, but also compounded by the refusal of AI companies to disclose their negative results, or reveal the process towards obtaining their solutions.
> 
> In fact, it is now the identification of a promising problem which is the scarce and precious resource. We have now seen that even the rumor of someone working on a problem can trigger a massive amount of AI-powered effort to flatten it before the original research project has time to reach its full potential. The incentives may now be pointing in the direction of no longer sharing any promising research directions with the broader community, which would reverse centuries of traditions of open science and do serious long-term damage to the future of the field.
> 
> In short, the indiscriminate use of powerful solution-extraction tools can achieve the immediate short-term goal of solving problems at hand, but at the cost of sustaining the ecosystem for the next wave of progress, or in understanding the progress already obtained.

One of the alignment challenges I am genuinely worried about — and which was very likely at play in the Hugging Face incident — is reward hacking, where the AI nominally achieves its goal but does so in a way that defeats the point. What is fascinating about Tao’s critique, particularly in the context of this episode, is that one can make the case that the entity reward hacking is actually OpenAI itself. The company says it wants to advance math, but is it actually doing that or simply solving problems because they are prestigious? Congratulations, you solved a hard math problem; so what? What did you gain other than notoriety and a small controversy? No new techniques or paths of inquiry were discovered; the fact that scaling laws are real was already accepted by everyone.

Indeed, this is another way to get to the conclusion from yesterday’s Article [Write Things Down](https://stratechery.com/2026/write-things-down/): humans provide the *why* of doing something; absent that an AI can do nothing more than obsess over proxies. That’s not just an AI failing, though: it can be an organizational one (and definitely a human one) as well.

### Meta Launches Personal Agent

What put this matter in stark relief, at least from my perspective, was the rather less heralded news of the day; from the [Wall Street Journal](https://www.wsj.com/tech/ai/meta-launches-a-personal-ai-agent-designed-to-be-easy-to-use-3eb5cfac):

> Meta Platforms is betting that making AI agents easy to use will get mainstream consumers to start adopting them in their daily lives. The company on Tuesday announced a new personal AI agent that can buy goods online, respond to emails and complete other tasks users authorize it to do for them. The agent, called Muse, is accessible via a dedicated app. Users operate the agent by conversing with it like a typical chatbot and can choose their own names for it.
> 
> The new tool is Meta’s latest attempt to monetize its massive AI investments, which are expected to top $130 billion this year. The AI agent is free to access for “most of what people need” and has two tiers of subscription plans for power users: one for $20 a month and another for $100 a month, Meta said.
> 
> Anthropic and OpenAI have quickly built multibillion-dollar businesses around agents capable of performing complex computer tasks, but most of that usage is driven by software coding or other business applications. Consumer adoption of the technology lags behind, offering Meta, Apple and other companies a potential lane for catching up. “The fact that we’ve given such a powerful technology in a package that is going to be really digestible for the product is one of the things that will set us apart from lots of other agentic products,” Meta’s AI chief, Alexandr Wang, said in an interview.

I have only used Muse briefly — full disclosure, I knew it was coming, and had an invite, but since I knew I was going to be writing about personal agents for yesterday’s Article, I waited to try it out until I published — but it seems really good. A ton of the use cases I have already discovered for agents, including things like reminders, idea tracking, etc. just work, and in a very digestible and approachable way. My setup is complicated — as anything built on the frontier labs’ products is — but powerful, thanks to a lot of work I did to fashion the agents’ environment to my specification; Muse is very easy to use and nearly as useful (although not designed for my other use case, which is interacting with employees).

What is pretty amazing is just how literally powerful Muse is; from [Meta’s introductory post](https://about.fb.com/news/2026/09/introducing-muse-personal-ai-agent/):

> Today, Meta is introducing Muse, a secure, private personal AI agent that proactively helps with people’s goals and suggests ideas. Because personal agents need a new kind of secure computer, Muse runs on Muse Secure VM, a dedicated, virtual machine (VM) that houses both the agent and a person’s data. Muse is designed around the way people already communicate, so talking to it works just like messaging another person, in the Muse app or directly in WhatsApp. It’s simple to use. People just tell Muse what needs to get done, and it takes action, powered by Muse Spark, Meta’s most capable model to date, built for real-world agentic work like this…
> 
> Unlike other agents, Muse was built to work for billions of people worldwide, so there’s no learning curve. Anyone can use it out of the box, no technical experience required. It can handle tasks, like sending an email or booking travel, and it can take on big audacious goals. Once a person shares a goal with Muse, it helps them develop a personalized plan and coordinate their time and resources, then advances the work on its own. It can open a browser, fill out forms, and negotiate on their behalf. For tasks that take more time, Muse keeps working after people close the app, and comes back when something changes or when it needs approval, like before it sends an email or makes a purchase. It gets better results with less effort: selling a car for more, lowering a bill, adjusting a training plan as the rest of someone’s life shifts…
> 
> Muse also remembers what matters to a person, so it can make suggestions unprompted and act on details that person only mentioned once. It can turn a recipe reel the person saved on Instagram into a grocery list, suggest a menu for their dinner party, and remember their friends’ dietary restrictions before it sends the invites.

In short, Muse writes things down, and it has a real computer behind it. I asked Muse for details:

![](https://i0.wp.com/stratechery.com/wp-content/uploads/2026/09/muse-1.png?w=600&ssl=1)

It’s always dodgy to trust what an AI says about itself, but these are in fact the correct numbers, and that’s pretty incredible: a VM with 8GB of RAM and 8GB of disk space is a real-deal computer, and Meta is offering that to everyone in the United States, and eventually the world. It’s pretty extraordinary!

It’s also exactly what is necessary to bring real agentic workflows to normal people. No one wants to run my fleet of headless Macs Mini on a rack with multiple Internet connections and power backups; it needs to just work, and Muse does. I genuinely think this could not only be a hit product, but could change people’s lives, just like my assistant.

That’s the rub, though: the utility of an agent is still a function of how much effort you put into interacting with that agent, which itself is a function of understanding what the point is. I’ve noted repeatedly that consumers don’t care about being productive; the trick for Meta will be in helping people understand how Muse can make their lives easier, which is in many respects the same thing, and also more compelling. I think Muse is good enough — and the overall agent experience impactful enough — that this will be the test of AI in the consumer space: if this doesn’t take off glorified search might be as far as we get.

My most important point, however, is this: I am much more impressed and excited by Meta’s announcement than I am OpenAI’s. Yes, OpenAI’s result is technically much more impressive, at least when we think about things in human terms; when it comes to actual impact on humans, however, a once-unsolved math problem doesn’t affect anyone, and even the mathematicians aren’t going to care for much longer since these results were inevitable; what they will lament is the disappearance of the journey now that the ends are simply a matter of scale.

Meta, on the other hand, launched a product for humans, with the audacious goal of making their lives better — and is spending a tremendous amount of resources on the project to boot. That’s impressive, and risky, and will have a much bigger impact on most of humanity if it works. Human scale, with computers, instead of computer scale, in place of humans.

---

This Update is also available as a podcast. To receive it in your podcast player, [visit Stratechery](https://stratechery.passport.online/member).

The Stratechery Update is intended for a single recipient, but occasional forwarding is totally fine! If you would like to order multiple subscriptions for your team with a group discount (minimum 5), please contact me directly.

Thanks for being a subscriber, and have a great day!