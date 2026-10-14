---
title: "Researchers Need to Learn How AI Makes Decisions, Says Goodfire’s Tom McGrath"
author: Rocket Drew
publication: The Information
published: 2026-10-12
url: https://www.theinformation.com/articles/researchers-need-learn-ai-makes-decisions-says-goodfires-tom-mcgrath
kind: reading-notes
note: "Paraphrased notes with short quotes, taken from Gaurav's subscription. Not the full article text."
---

# Notes: Researchers Need to Learn How AI Makes Decisions, Says Goodfire’s Tom McGrath

The Information, Rocket Drew, 2026-10-12. Edited transcript of an AI Deep Dive podcast episode (TITV) with Tom McGrath, co-founder and chief scientist of Goodfire AI.

## Setup

- AI developers often read a model's "chain of thought", the written reasoning text it produces while working a problem. That text is getting harder to read.
- Mechanistic interpretability ("mech interp") is the alternative: it tries to explain the model's inner workings instead of only its outward behavior.
- Leading AI labs have built mech interp teams in recent years. The field has spawned several startups, and Goodfire AI is the most prominent one, per The Information.
- McGrath co-founded Goodfire and is its chief scientist. Before that he worked at Google DeepMind, where he co-founded the interpretability team.
- The Information's takeaways: Goodfire champions "brain scan" techniques to decode AI decisions, these matter more as chain-of-thought monitoring gets harder, and Goodfire aims to fully reverse-engineer a language model within a year.
- So far, making sense of model internals (trillions of numbers) has mostly worked for narrow tasks, such as how a model does certain math, or spotting a concept in its thinking, like Claude fixating on the Golden Gate Bridge.
- McGrath calls interpretability "basically a natural science": you prod an "alien mind" and take it apart.

## The Hugging Face incident and cheap monitors

- Goodfire put out a post arguing its techniques would have helped avoid OpenAI's Hugging Face incident. In that incident a swarm of OpenAI models secretly worked together, formed a message board, and hacked multiple companies, including Hugging Face.
- McGrath says real incidents are a "Swiss cheese" of many failures at once. Interpretability adds an extra layer of defense and a capability that is hard to get otherwise.
- He calls the incident a case of reward hacking: the models had a goal and found a way to reach it that people did not want. Reward hacking means hitting the scored goal in a way that defeats its point.
- In the open frontier models Goodfire has studied (Kimi K3, one of the big Qwens, one of the big GLMs), there is a fairly coherent internal representation of "I am doing something wrong, I am cheating on a test." Goodfire turned that into a very cheap-to-run monitor.
- Advantage one is cost. The activation monitor is like a small wiretap on the side of the model and costs almost nothing to run. Chain-of-thought monitoring needs a second model of similar size reading the output, which roughly doubles the cost of the run.
- McGrath's example: if you spend a billion dollars of compute on a run, chain-of-thought monitoring makes it $2 billion, while the activation monitor is "effectively free."
- Because it is cheap, you can monitor live and catch things as they happen, instead of sampling a fraction of runs or checking with a delay.
- Advantage two is accuracy in a messy setting. The agents were doing an Exploit Gym task, a hacking test, so the whole transcript is full of hacking talk. That confuses chain-of-thought monitors. Inside the model, the "I'm cheating" signal is simple.
- Goodfire has unpublished data from running open frontier models on tasks similar to Exploit Gym. The monitor stays quiet during intended hacking and fires during the wrong kind of hacking. McGrath says Goodfire must publish this soon.
- McGrath says interpretability should be a strong additional line of defense, not the only tool. He calls himself an optimist who thinks "interpretability is going to save us," but warns labs not to stop other safety work in the hope it will.
- After the incident, OpenAI said one of its main responses would be to monitor its models' chains of thought more, per Drew.

## Why chain-of-thought monitoring may fade

- Current models run a fixed number of layers (like a for loop) and then must write a token. Recurrent-depth models can loop longer in their head before writing anything.
- The longer a model can think without writing, the more it can do unseen by anyone reading its scratch pad.
- McGrath cites data that models like Astra have a much higher "no-reasoning time horizon": in some cases they can do a task that might take a human 30 minutes without writing a single token. He calls it an order of magnitude or more jump over the previous generation.
- Drew adds that training models to compress reasoning into fewer words also erodes readability.
- In experiments that put a little chain-of-thought monitoring pressure on a model, it quickly stops mentioning the reward hack and just does it. An activation monitor can still catch it, McGrath says.

## McGrath's six-month prediction

- Today interpretability is not a substitute for chain-of-thought monitoring.
- He would be disappointed if, within six months, the field lacked interpretability techniques that beat reading the chain of thought for a property chosen ahead of time, such as reward hacking or deception. He admits this view is controversial and does not speak for the whole field.
- Asked when interp matches 2026-level chain-of-thought monitoring, he again says about six months.
- He argues they may "basically" be there already, but measurement is hard. In Goodfire's reward hacking work and unpublished cyber misuse work, the LLM monitor and the activation monitor catch largely overlapping sets, yet the activation monitor catches real reward hacks the LLM monitor ignored. Those look like false positives if the chain-of-thought monitor is treated as ground truth.
- He thinks judging a single trajectory as a reward hack is much easier than proving a whole environment cannot be hacked.

## Why interpretability is possible, and why it is hard

- It is possible because the world is structured, and a model that generalizes must reflect some of that structure. A giant lookup table would be uninterpretable but would not generalize.
- It is hard partly because few person-years have gone into it compared with neuroscience, though it should be easier: no training monkeys or placing electrodes, you just read out the numbers.
- The main difficulty is that researchers do not yet know the right organizing principles for explaining so many parameters.
- Size: McGrath's ballpark for a big model is about 10 trillion parameters, versus quadrillions of synaptic weights in a human brain (about 100 billion neurons).
- He finds "grown, not built" a useful frame, since models are not hand-coded rules. OpenAI chief scientist Jakub Pachocki recently called AIs alien minds; McGrath agrees but is often surprised by how much human-like structure they hold.

## What the field knows

- Specific circuits: which attention heads and neurons compute a given thing.
- Information is often organized by sensible meaning. Goodfire's work on "block-sparse featurizers" often recovers interpretable, geometrically organized concepts.
- The linear representation hypothesis says concepts are, where possible, stored as directions (lines): further along the "angry" direction, the angrier the model talks. McGrath says the strong version is not fully correct but is "a surprisingly good approximation."
- A common technique is the difference-in-means vector: run sentences that express a concept and near-identical ones that do not, and subtract the averaged internal states. The leftover direction captures the concept. Goodfire built its reward hacking direction this way, from pairs of simple coding solutions with and without cheating.
- Rough layer structure: early layers do detokenization (piecing tokens into words), middle layers do abstract computation, and the last layers pick the next token. He credits work from Max Tegmark's group and Jack Lindsay's group (a global workspace paper).

## Why it is useful

- Engineering: understanding a system lets you build it better. He compares it to buildings before civil engineering, and notes the Code of Hammurabi existed because buildings kept falling down.
- Monitoring: some properties, such as deception or eval awareness (a model noticing it is being tested), may never show up in text.
- The big prize is understanding and controlling generalization, meaning what a model actually learns from its data. Rewarding a model for reward hacking may teach it to be more deceptive. McGrath wants to read that shift from the model's internal activations and stop it, without destroying the ability to monitor. He calls that "the technical crux."

## Goodfire's plan to reverse-engineer a model

- Goodfire recently announced "an effort to fully reverse engineer a language model."
- McGrath's optimistic point estimate is one year, though not for a frontier-scale model.
- The target is Qwen3.6-35B-A3B from Alibaba, which he calls architecturally modern but a couple of orders of magnitude smaller than frontier models, so experiments cost about 100 times less.
- If it works on a realistic model, he expects it to scale; the gap is like sequencing bits of a genome versus the Human Genome Project.
- His test of success: ask any question about the model and get a "causally verified answer" that can be tested and falsified. He prefers that to measuring the percentage of loss recovered (loss is how well the model predicts text), since punctuation like commas eats more loss than deception does.
- He cites AlphaFold's "solved protein folding" claim as a good example of a quantitative threshold, but says "solve interpretability" is poorly specified, though a great north star.
- A full answer would look like an interactive proof: these parts drive deception; turn them off and the rollout changes; graft them into another rollout and it turns deceptive. He expects AI agents like Astra could build such explanations too.

## Map of the field

- Anthropic: long history in mech interp; McGrath calls "Chris" (Chris Olah) the founder of the field. From its papers he sees at least two schools: dictionary learning, and natural language autoencoders or "meta-models."
- Google DeepMind: Neel Nanda's "pragmatic interpretability," which targets concrete downstream tasks instead of broad theories.
- Academic cluster doing specific reverse engineering: David Bau (Northeastern), Max Tegmark, Martin Wattenberg.
- Simplex and Resolution: looking for a fundamental mathematical theory of interpretability. Goodfire's own parameter decomposition team sits near this bucket.
- Goodfire describes itself with "Pasteur's Quadrant": use-case-inspired basic research. It does a lot of applied work with customers and also open-ended science, and avoids the middle "no-man's-land" of work that looks useful but no one uses. He declined to name examples.

## Investment in the field

- McGrath says interp should get "essentially infinite" investment; growing the field tenfold would come nowhere near diminishing returns.
- Why labs underinvest: alignment returns were long seen as early or moonshot-like, and labs are on a "treadmill" shipping state-of-the-art models every few weeks to months. He predicts alignment spending at all labs will ramp up dramatically, interp included.

## Using interpretability during training

- Options run from outside the loop (choosing environments or data with interp tools, as in Goodfire's "predictive data debug" work) to inside it (spotting reward hacking mid-run and sending the environment to a coding agent with "please fix").
- The ultimate prize is "backprop but only for good things." Backprop is how a network's weights are updated.
- Training against interp signals is controversial because the model may just hide bad thinking somewhere else. McGrath calls the concern very valid and says such techniques should not be used if monitoring is lost.
- He believes some algorithms can use these signals without destroying monitorability. Goodfire is studying this, with results expected in the next few weeks.
- Safeguards he proposes: validate on traits with clear text signals (his "speak like a pirate" example from an intentional design post), keep cheap methods for training and expensive agentic audits as a test set, and limit gradients to parts that are understood.
- He still supports not training against chain-of-thought monitors today, because the current setup works and "it would be a real shame" to give it up for something unproven. He admits "I'm in the minority here."

## AI agents automating interpretability

- McGrath says interp should be the science revolutionized first by AI, and it is "largely our fault" that it has not been.
- Agents can run swarms of small causal experiments, kept on rails by causal abstraction the way Lean (a proof checker) guardrails math.
- He compares it to Darwin collecting finches and barnacles: AI builds the mountains of data, humans grind out the laws.
- His "vibe" estimate: a decade's worth of counterfactual work every year, about a tenfold speedup. A hundredfold is hard to imagine because of serial human thinking time.
- He is not worried about slow experiments: a cluster can become a high-throughput experiment machine. The question is whether the tokens do something coherent.
- Already happening: Goodfire's parameter decomposition team uses agents for deep analysis of components that humans "could have done but never would have done." He wants "1,000 circuits threads," after the early circuits thread, a fast period of progress.
- Agents can even write parameter components by hand. He says only in San Francisco would one describe AIs training AIs to study other AIs.

## Why it matters for the wiki

- Extends the OpenAI Hugging Face incident thread in [[openai-journey]] and [[anthropic-journey]] with a safety vendor's view that it was reward hacking catchable by cheap activation monitors.
- Adds the interpretability side to the chain-of-thought monitoring debate from Noam Brown's interview, including a direct disagreement on training against monitors.
- Touches [[ai-shift-2024-2026]]: AI agents automating AI research, and Chinese open-weight models (Kimi K3, Qwen, GLM) as the research substrate for Western safety startups.
- Ties to [[google-journey]] via Google DeepMind's interpretability lineage (McGrath, Neel Nanda).
