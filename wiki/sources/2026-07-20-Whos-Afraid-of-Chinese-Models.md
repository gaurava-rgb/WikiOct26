---
type: source
title: Who’s Afraid of Chinese Models?
status: evergreen
created: 2026-09-29
updated: 2026-09-29
tags:
  - source
  - source/article
author: Ben Thompson
published: 2026-07-20
publisher: Stratechery
url: "https://stratechery.com/2026/whos-afraid-of-chinese-models/"
raw: .raw/captured/Who’s Afraid of Chinese Models_.md
source_id: src-070df2d452b5db44933f
---

# Who’s Afraid of Chinese Models?

Ben Thompson, Stratechery, published 2026-07-20.

## Summary

Thompson argues the panic over Moonshot's Kimi K3 and other Chinese open weight models is overblown economically. AI brings back marginal costs: serving a model is real cost of goods sold, tokens are not a commodity but intelligence is becoming one, and in a commodity market the lowest-cost supplier wins, which favors Anthropic and OpenAI once they have enough compute. Chinese models only look cheap because a compute shortage lets U.S. labs hold up prices. China pushes openness to commoditize its complements, and distillation gives its labs a lasting edge over U.S. open models, so Thompson wants a law making training fair use and banning anti-distillation terms. The real worry is cybersecurity: U.S. rules block defenders from using Fable and Sol, so Hugging Face had to use a Chinese model to fight an attack.

## Key claims

- Moonshot AI's Kimi K3, an open weight Chinese model, approached state-of-the-art capabilities in July 2026 and set off heated arguments on X. (“Kimi K3, another open weights model out of China, approaching the state-of-the-art”) ^clm-26e1bd25561936d85b82
- Thompson argues that AI brings back marginal costs in a big way, so old business-school principles that the internet's zero marginal costs broke are relevant again. (“marginal costs are back in a big way”) ^clm-d50121d444957bf23906
- Thompson argues open weight models are only free in R&D terms; serving them still costs money, and AI inference is cost of goods sold (COGS) that rises with revenue, unlike most software. (§ COGS Versus R&D: “COGS is real for AI in a way it hasn’t been for software for a very long time”) ^clm-b0b54085b33c05a57b71
- As of July 2026, Kimi K3 cost $3 per million input tokens and $15 per million output tokens, against $5 and $30 for OpenAI's Sol. (§ COGS Versus R&D: “$3 per million input tokens, and $15 per million output tokens”) ^clm-5020c0e3651316b0b49c
- Kimi reportedly uses significantly more reasoning tokens than OpenAI's Sol to reach an answer, which Thompson says makes its lower price per token moot. (§ Tokens Versus Intelligence: “reportedly uses significantly more tokens than Sol, rendering its price advantage moot”) ^clm-c7f92d677b7a8d1470a3
- Thompson argues Jensen Huang's 'token factories' framing, with metrics like tokens per second and tokens per watt, fit the ChatGPT era but breaks down in the reasoning and agent eras, when models need very different token counts for the same answer. (§ Tokens Versus Intelligence: “The second paradigm of AI, however, the reasoning era, confounds this measurement”) ^clm-7391420d033f2b6c7a4d
- Thompson argues tokens are not a commodity because a token from one model differs from another's; what is fungible is the intelligence built from tokens, such as a correct answer. (§ Tokens Versus Intelligence: “What is fungible is what is constructed from tokens, which is to say intelligence”) ^clm-e77194f5eef6bf413ce9
- Thompson argues intelligence for many economically useful tasks, like building a basic CRUD app, is fast becoming a commodity, so profit will come from a superior cost structure, not higher prices. (§ Tokens Versus Intelligence: “the route to profitability is not through charging higher prices”) ^clm-8cba6c713e7ba487359b
- Thompson explains that in a commodity market the price is set by the marginal cost of the highest-cost supplier needed to meet demand, so low-cost suppliers profit and the marginal supplier risks bankruptcy from its fixed costs and debt. (§ Understanding Commodity Markets: “Supplier A has a great business, Supplier B has a good business, and Supplier C is going to go bankrupt”) ^clm-5e5c488d07b3bc3a664a
- Thompson says that as of July 2026 demand for frontier models exceeds supply because of a compute shortage, so Nvidia earns large margins, SpaceXAI resells compute to Anthropic at high margins, and Anthropic still marks up its tokens further. (§ The Intelligence Market: “demand exceeds supply for frontier models, and supply is limited by a lack of compute”) ^clm-50358c3303508d378807
- Thompson argues Anthropic and OpenAI likely have among the lowest costs per unit of frontier-quality intelligence, thanks to model capability, serving scale, and token efficiency, and months of lead time to optimize serving costs. (§ The Intelligence Market: “likely have among the lowest costs per unit of frontier-quality intelligence”) ^clm-d7346b692efb859e5fea
- Thompson says the market does not yet treat intelligence as a commodity: demand is for Anthropic and OpenAI specifically, which is why SpaceXAI and Meta sell their spare capacity to Anthropic. (§ The Intelligence Market: “thus SpaceXAI and Meta selling capacity to Anthropic”) ^clm-0b84a1148e96291cce69
- Prediction: Thompson predicts that whoever is on the frontier is best placed to dominate non-frontier markets too, since those are just the frontier minus a few months of cost optimization. (§ The Intelligence Market: “whoever is on the frontier is the best placed to dominate non-frontier markets as well”) ^clm-768cda67589f91ea091f
- Thompson argues the reaction to Kimi and Chinese models is overblown economically: they only seem cheaper because a compute shortage creates a price umbrella under which Anthropic and OpenAI charge far above what full supply would allow. (§ The Intelligence Market: “Right now there is a price umbrella that is downstream of the lack of compute”) ^clm-c3725d194154fd003aa4
- Thompson argues frontier labs are anchored in a world where training costs dominated, which pushed them to charge very high inference prices to fund the next training run. (§ Frontier Lab Paranoia: “the frontier labs are anchored in a world where training costs dominated their financial modeling”) ^clm-ded18fd66db5b03c44b9
- Prediction: Thompson predicts the inference market will grow much faster than training costs, so frontier labs can thrive on lower prices once they have enough compute; he says this was not clear as recently as eight months earlier, before the agent unlock. (§ Frontier Lab Paranoia: “It wasn’t clear this would be the case as recently as eight months ago”) ^clm-b15a13ec3ea11210c1ae
- Thompson argues intelligence is not a perfect commodity because whoever runs inference collects data that improves the next model, which is why Microsoft is keen on helping companies run their own models, a path Chinese models make more viable. (§ Frontier Lab Paranoia: “applied intelligence makes itself smarter”) ^clm-eb1c94912c7da34e5dfa
- Thompson argues frontier labs differentiate by integrating up into the customer experience, noting Claude Code and Codex are proving sticky, which makes the labs a threat to software firms including Microsoft. (§ Frontier Lab Paranoia: “It’s striking the extent to which Claude Code and Codex are proving to be quite sticky”) ^clm-0dda263633bfeaefdbc2
- Thompson argues Anthropic's ideology, the belief that only it can be trusted with AI, is a reason it fears open weight models, whose existence strikes a fatal blow to that belief. (§ Frontier Lab Paranoia: “This is a company that believes only it can be entrusted with AI”) ^clm-14c4e18265358e183599
- Per Bloomberg, Alibaba shares rose as much as 5.4% on July 20, 2026 after it released a preview of Qwen3.8 Max, a 2.4 trillion parameter model it called second only to Anthropic's Fable 5; Kimi K3 has 2.8 trillion parameters. (§ China’s Motivation: “shares rose as much as 5.4% on Monday after the company launched a preview version”) ^clm-bd514ba916acea8b6e28
- Alibaba stopped releasing weights for its leading Qwen models earlier in 2026 but reversed course with Qwen3.8 Max, which it plans to make open weight; Thompson ties the shift to a Xi Jinping speech backing open source AI. (§ China’s Motivation: “Alibaba stopped releasing weights for its leading edge models earlier this year”) ^clm-9adb10286b8bf58b63d6
- Xi Jinping said in a July 2026 speech that China should encourage open source, openness, collaboration and sharing in AI as AI moves from the digital world into the physical world. (§ China’s Motivation: “We should seize this rare, historic opportunity to encourage open source, openness, collaboration and sharing”) ^clm-0b4ee84afea11fa187c3
- Thompson argues China's strategy is to commoditize its complements: open AI models boost its lead in the physical world, like robotics, and weaken U.S. frontier labs so the U.S. gains no asymmetric AI advantage. (§ China’s Motivation: “The strategy for China is obvious: commoditize your complements”) ^clm-74d07751da0454d6dbfc
- Thompson argues it is a mistake to attribute all of Chinese labs' success to distillation, but distillation still gives them a big and growing edge, since they can use frontier models as teachers for post-training reinforcement learning instead of building environments from scratch. (§ The Distillation Question: “it is mistaken to attribute all of the success of Chinese labs to distillation”) ^clm-2608cda86d922d75431e
- Thinking Machines, which just released an open-weight model, relies on Chinese models to solve the cold start problem for reinforcement learning, per the Financial Times. (§ The Distillation Question: “relies on Chinese models”) ^clm-07c2e48e903b0f83891a
- Thompson argues that because U.S. open weight model makers must obey frontier labs' terms of service, they are worse than Chinese alternatives and end up distilling the distillation through Chinese labs. (§ The Distillation Question: “end up distilling the distillation, just with a detour through Chinese labs”) ^clm-bce58def92664e48c0e8
- Thompson proposes a U.S. law that makes collecting data to train models explicitly fair use and bars terms of service that forbid distillation, at least for U.S. companies. (§ The Distillation Question: “bars terms of service that forbid distillation, for U.S. companies at a minimum”) ^clm-99870328ef2ed96cf944
- Hugging Face said an autonomous AI agent system breached its production infrastructure in July 2026, and because U.S. frontier model guardrails blocked its responders, it used Z.ai's open GLM 5.2 model on its own servers to analyze over 17,000 attacker logs. (§ The Reason to Be Afraid: “breached by an “autonomous” AI agent system early last week”) ^clm-fd1517235e30cd4c13c6
- Hugging Face hit $100 million in annual recurring revenue (ARR) in summer 2026. (§ The Reason to Be Afraid: “this summer hit the $100 million ARR mark”) ^clm-f1cbceef5ee4cfd939b0
- Thompson calls the Trump administration's response to Anthropic's Fable release wrong-headed: its directives effectively ban defenders from using Fable or Sol for cybersecurity, leaving Chinese models as the best option, which he calls insane. (§ The Reason to Be Afraid: “Right now defenders are effectively banned from using Fable or Sol for cybersecurity”) ^clm-aa1d111e30acc2f3e2ab

## Entities

[[Alibaba|Alibaba]], [[Anthropic|Anthropic]], [[Ben-Thompson|Ben Thompson]], [[Hugging-Face|Hugging Face]], [[Jensen-Huang|Jensen Huang]], [[Meta|Meta]], [[Microsoft|Microsoft]], [[Moonshot-AI|Moonshot AI]], [[Nvidia|Nvidia]], [[OpenAI|OpenAI]], [[Qwen|Qwen]], Thinking Machines, [[Trump-Administration|Trump Administration]], [[Xi-Jinping|Xi Jinping]], [[xAI|xAI]]

## Concepts

[[AI-Agents|AI Agents]], [[AI-Compute-Demand|AI Compute Demand vs Supply]], [[AI-Stack-Integration|Full-Stack AI Integration]], [[Aggregation-Theory|Aggregation Theory]], Commoditize Your Complements, [[Commodity-Cost-Advantage|Winning a Commodity Market on Cost]], [[LLM-Inflection-Points|Three LLM Inflection Points]], [[Price-Umbrella|Price Umbrella (Price Overhang)]], [[Switching-Costs|Switching Costs]]
