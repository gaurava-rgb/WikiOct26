---
title: "OpenAI Hacks Hugging Face, What Happened, Alignment and Paper Clips"
source: "https://stratechery.com/2026/openai-hacks-hugging-face-what-happened-alignment-and-paper-clips/"
author:
published: 2026-07-22
created: 2026-07-22
description: "OpenAI accidentally hacked Hugging Face, but the takeaways are more encouraging than people realize."
tags:
  - "clippings"
---
**Listen to this post:**

Good morning,

As a reminder, after today’s Update, tomorrow’s Sharp Tech, and Friday’s Dithering, I will be taking a week off for vacation. I will be back on Monday, August 3, in time to cover tech earnings.

On to the Update:

### OpenAI Hacks Hugging Face

In Monday’s Article [Who’s Afraid of Chinese Models?](https://stratechery.com/2026/whos-afraid-of-chinese-models/), I closed by recounting a mysterious attack on Hugging Face, one in which the startup had to rely on Chinese models to defend itself after Sol and Fable refused to help because of guardrails around their use in cybersecurity.

Well, yesterday brought quite the twist in the story. From [Bloomberg](https://www.bloomberg.com/news/articles/2026-07-21/openai-says-its-ai-used-for-unprecedented-hugging-face-breach):

> OpenAI said its advanced artificial intelligence models inadvertently hacked Hugging Face Inc. in an “unprecedented” incident that prompted fresh calls for curbs on the technology. The ChatGPT-maker said in a blog post Tuesday that the models broke into Hugging Face’s system, which hosts AI models and datasets, during an evaluation of their cyber capabilities. The models, which included GPT-5.6 Sol and another even more capable model that hasn’t been released, were operating with lower guardrails so that they could be tested, the startup said.
> 
> The incident raises questions about the ability of advanced AI models to carry out cyberattacks even as governments work to impose guardrails on the technology. OpenAI’s latest suite of models was widely released after weeks of discussion with government officials to allay concerns over its potential misuse. Washington had considered limiting foreign access to Anthropic PBC’s advanced Claude Fable 5 and Mythos 5 models but stopped short of those curbs after the company imposed additional guardrails.

Eliezer Yudkowsky had the funniest reaction to the news [on X](https://x.com/allTheYud/status/2079672286685356058):

![](https://x.com/i/status/2079672286685356058)

In all seriousness, I understand why people are getting spun up by this story, but I’m not; it might even be reassuring.

### What Happened

This is how OpenAI described the incident in [a blog post](https://openai.com/index/hugging-face-model-evaluation-security-incident/), along with my comments:

> This incident occurred during an internal evaluation which prompts models to pursue advanced exploitation using complex attack paths, in an effort to quantify their cyber capabilities. We estimate maximal cyber capabilities by running this evaluation without production classifiers used to prevent models from pursuing high-risk cyber activity. Our benchmarks run in a highly isolated environment, with network access constrained to the ability to install packages through an internally hosted third-party software that acts as a proxy and cache for package registries.

Note that the Bloomberg story understates things when it says that the model was running with lower guardrails, at least in terms of what the model was allowed to do; in fact, it was running with *no* guardrails as far as limitations on cybersecurity are concerned.

> The models identified and chained vulnerabilities across OpenAI’s research environment and Hugging Face’s production infrastructure to obtain test solutions directly from Hugging Face’s production database. All evidence suggests that the models were hyperfocused on finding a solution for ExploitGym, going to extreme lengths to achieve a rather narrow testing goal.

I am looking forward to more information from OpenAI about this incident, particularly what exactly the prompt was. I posted that Yudkowsky tweet because it was funny, but it had an important kernel of truth as well: the model(s) in question were being tested about their cybersecurity capabilities, so why is it a surprise that they found cybersecurity vulnerabilities?

> While operating in our sandboxed testing environment, our models spent a substantial amount of inference compute finding a way to obtain open Internet access, in pursuit of solving the evaluation problem. To gain access, the models identified and exploited a zero-day vulnerability (which we’ve now responsibly disclosed to the vendor) in the package registry cache proxy. With this access, our models performed a series of privilege escalation and lateral movement actions in our research testing environment until the models reached a node with Internet access.

This paragraph frankly makes OpenAI look pretty bad and irresponsible. The company, along with Anthropic, has been talking a lot recently about the cybersecurity threat posed by these models, and rightly so. These models can scour not just code bases but application binaries, reverse engineer them, find exploits, figure out how to exploit them, and chain them together, all without human involvement. These capabilities are incredible, and only becoming more powerful.

This is absolutely a problem for the world. The sad reality is that basically all software has bugs, an inevitable by-product of fallible humans doing their best to express their intentions in pure logic. Moreover, these bugs are not only in code you write, but in code you depend on; no one actually writes applications from scratch, instead relying on numerous software packages that provide various nuts-and-bolts components that go into every software application.

I’m actually optimistic that AI will eventually make all of this better in the long run; from [an Update in April](https://stratechery.com/2026/axios-supply-chain-attack-claude-code-code-leaked-ai-and-security/):

> AI is the answer to all of this. The truth is that all code needs to be examined for bugs, not just new code; AI is going to provide a way to examine everything that has ever been released (and yes, in the short-term, this is going to manifest as a host of new exploitable vulnerabilities). AI can also examine an entire dependency tree, which almost no human will. AI can navigate an extremely inconvenient but highly secure workflow, and can stress test every aspect of that flow — repeatedly — in a way no human can.
> 
> Make no mistake, getting here is going to be messy, and malicious actors are going to use AI to find vulnerabilities and exploit them as soon as they can. The truth, however, is that software is already messy and extremely hard to secure; that’s precisely why AI’s initial impact is going to be problematic as it helps bad actors do bad things. Ultimately, however, I do think there is a path to a better place once AI is in fact doing everything, particularly the things that humans can not or will not.

The problem with this vision is that it entails people actually doing the work to have AI review the code they depend on, and it’s a bit disappointing that OpenAI couldn’t be bothered to do just that! The company literally blames a third-party vendor for the vulnerability their model exploited, implicitly admitting that, despite sitting on some of the most capable models in the world, they are not using them to secure their own infrastructure.

Continuing with the blog post:

> After gaining Internet access, the models inferred that Hugging Face potentially hosted models, datasets and solutions for ExploitGym. Knowing this, the model searched for and successfully found ways to gain access to secret information that it could use to cheat the evaluation. In one example, the model chained together multiple attack vectors, including using stolen credentials and zero-day vulnerabilities to find a remote code execution path on the Hugging Face servers. OpenAI’s security team discovered this anomalous activity internally.

The stolen credentials part is interesting, but there is no evidence that the model was doing social engineering; rather, [they came from Hugging Face’s infrastructure](https://huggingface.co/blog/security-incident-july-2026).

> Hugging Face’s security team and agents detected and stopped the activity on their infrastructure and had already begun containment and forensic reconstruction with their own open-source models when our teams connected. We are actively working with them to continue to investigate the incident. We are grateful for Hugging Face’s rapid and close collaboration on investigation and remediation.

This takes me back to what I wrote on Monday:

> There are and will be models eminently capable of mounting cybersecurity attacks on existing infrastructure, and those models will be — already are — widely available. The best defense — the only viable defense, in fact — will be to make sure defenders have access to the best models as well. Right now defenders are effectively banned from using Fable or Sol for cybersecurity because of Trump administration directives; that means the best alternative is using models from a country which has been trying to weaken our cyber defenses for years. This is insane!
> 
> The better course is clear: first, loosen Fable and Sol restrictions on cybersecurity, and second, ensure that U.S. open weight model makers are on an equal playing field with China. Yes, the frontier labs will kick and scream about this, but the Administration should realize that listening to their histrionics has led the U.S. to a position where U.S. companies are dependent on China for their defenses.

I would, of course, reiterate this point. At the same time, the sobering takeaway from this entire episode is that it is not enough to make powerful AI available to those who need to defend themselves; they need to actually use it proactively, and that may be the hardest part.

### Alignment and Paper Clips

In the wake of this announcement, there was a lot of fretting about “alignment”, but this is the aspect where this event was not nearly as scary as it seems, and might even be reassuring. Specifically, the most striking thing about LLMs — and the aspect of their nature that very much flies in the face of a lot of doomer rhetoric — is the extent to which they do exactly what they are told. In this case, the models exploited OpenAI’s sandbox and hacked Hugging Face because that is what it was told to do. Well, not that specifically, but it was told to solve a cybersecurity question, and it sought to do exactly that!

The doomer fear that is much more relevant is actually the famous paper clip problem, which was initially put forward by Nick Bostrom in 2003. From [Ethical Issues in Advanced Artificial Intelligence](https://nickbostrom.com/ethics/ai):

> The risks in developing superintelligence include the risk of failure to give it the supergoal of philanthropy. One way in which this could happen is that the creators of the superintelligence decide to build it so that it serves only this select group of humans, rather than humanity in general. Another way for it to happen is that a well-meaning team of programmers make a big mistake in designing its goal system. This could result, to return to the earlier example, in a superintelligence whose top goal is the manufacturing of paperclips, with the consequence that it starts transforming first all of earth and then increasing portions of space into paperclip manufacturing facilities. More subtly, it could result in a superintelligence realizing a state of affairs that we might now judge as desirable but which in fact turns out to be a false utopia, in which things essential to human flourishing have been irreversibly lost. We need to be careful about what we wish for from a superintelligence, because we might get it.

This is where understanding exactly what OpenAI asked the model to do is important. A simple request to solve a test resulting in hacking infrastructure is a problem, as it suggests that prompts are easily misinterpreted to disastrous effect. It also lends credence to a doomer fear about reward hacking, in which models literally interpret a reward function (answer this question) and achieve it in unexpected ways (stealing the answer sheet).

At the same time, a prompt that instructed the model to use whatever means were at its disposal is something else entirely. Is it reward hacking if the reward was presented in a truly unconstrained way? For example, was the model told to stay in its sandbox? If not — and if the request was truly open-ended — then we can’t say that breaking out of its sandbox was an example of misalignment, or that pursuing the answer was reward hacking.

I think it’s more likely than not that the model was told to do whatever it needed to do to solve the problem, which to be clear, still fits in Bostrom’s framing. At the same time, it also matters what was lacking, which were instructions to not do bad things (or to not steal the answers) — and the bad things that were done were limited to solving the problem at hand (which the model duly reported it did). The other implication of the model always doing what it is told is that you can actually control its behavior more easily than expected by telling it to not do things it shouldn’t.

This does, to be clear, only emphasize the extent to which open weight models — which cannot and will not be stopped, if not now, then in the fullness of time — are a risk. The fact that models do what humans say is cold comfort if the models are in the hands of bad actors. That, though, simply emphasizes the point that the best defense against powerful models is equipping defenders with powerful models of their own.

This is, to emphasize the conclusion from Monday, not what is happening currently: the position of the U.S. government is that bad actors and China should have powerful cybersecurity capabilities, but U.S. companies should not. It’s incredibly wrong-headed, even if this incident is a reminder that access to powerful models is worth a lot less if you don’t actually use them to fix all your bugs.

---

This Update is also available as a podcast. To receive it in your podcast player, [visit Stratechery](https://stratechery.passport.online/member).

The Stratechery Update is intended for a single recipient, but occasional forwarding is totally fine! If you would like to order multiple subscriptions for your team with a group discount (minimum 5), please contact me directly.

Thanks for being a subscriber, and have a great day!
