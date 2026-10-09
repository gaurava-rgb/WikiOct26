---
type: source
title: An Interview with OpenAI CEO Sam Altman and AWS CEO Matt Garman About Bedrock Managed Agents
status: evergreen
created: 2026-09-29
updated: 2026-09-29
tags:
  - source
  - source/interview
author: Ben Thompson
published: 2026-04-28
publisher: Stratechery
url: "https://stratechery.com/2026/an-interview-with-openai-ceo-sam-altman-and-aws-ceo-matt-garman-about-bedrock-managed-agents/"
raw: .raw/captured/An Interview with OpenAI CEO Sam Altman and AWS CEO Matt Garman About Bedrock Managed Agents.md
source_id: src-11caadea4b839f865bfd
---

# An Interview with OpenAI CEO Sam Altman and AWS CEO Matt Garman About Bedrock Managed Agents

Ben Thompson, Stratechery, published 2026-04-28.

## Summary

OpenAI and AWS launched Bedrock Managed Agents, powered by OpenAI: OpenAI models packaged with AWS tools for identity, permissions, and security so companies can run agents inside their own AWS account. It came one day after Microsoft and OpenAI changed their deal so OpenAI can sell on any cloud. Altman says the harness (the software around the model) and the model are merging, and that demand for cheap intelligence has no ceiling. Garman says AWS wins by partnering with many model makers instead of owning the whole stack like Google. It matters because OpenAI models were long locked to Microsoft Azure, which helped rival Anthropic win enterprise buyers who stay on AWS.

## Key claims

- On 2026-04-27 Microsoft and OpenAI amended their deal so OpenAI can serve all its products on any cloud provider, including AWS; Microsoft stays the primary cloud partner and products ship first on Azure. (“OpenAI can now serve all its products to customers across any cloud provider”) ^clm-3912d088973d129a218b
- Under the new deal Microsoft keeps a license to OpenAI models and products through 2032, but the license is now non-exclusive. (“license to OpenAI IP for models and products through 2032”) ^clm-bf11d810f08b2490979b
- Microsoft no longer pays a revenue share to OpenAI; OpenAI's revenue share payments to Microsoft continue through 2030 at the same percentage but with a total cap. (“Revenue share payments from OpenAI to Microsoft continue through 2030”) ^clm-cc8e40aad2f8d330b062
- OpenAI released Microsoft from the AGI clause (a term that could end the deal once OpenAI reached human-level AI), so the agreement runs through 2032 no matter what. (“now the agreement between the two companies will run through 2032 no matter what”) ^clm-216dedabf6ebb743cc36
- Thompson argues Azure's exclusive hold on OpenAI models was hurting Microsoft's investment in OpenAI, because enterprises want models on the cloud they already use, which helped Anthropic grow. (“Azure’s exclusivity was actively damaging Microsoft’s investment in OpenAI”) ^clm-668b4b337ea46e815a22
- Thompson argues OpenAI sees AWS as so big an opportunity that it gave up Azure-related revenue for the next few years to get there. (“they are forgoing Azure-related revenue for the next few years”) ^clm-2ba4e3f00655a4d28e89
- Thompson describes Bedrock Managed Agents, powered by OpenAI, as Codex in AWS: OpenAI frontier models packaged inside an AWS-native agent runtime with identity, permissions, logging, governance, and deployment. (“The easiest way to think about this offering is Codex in AWS”) ^clm-6f9f326aee5a1266959b
- Garman says the vast majority of scaling startups still grow on AWS, citing scale, availability, security, reliability, and the partners and customers already there. (§ AWS and Startups: “the vast majority of scaling startups are still scaling on AWS today”) ^clm-281f51f7e1298bedbd62
- Garman agrees that a common startup pattern is AWS for regular computing plus the OpenAI API directly for AI. (§ AWS and Startups: “I think that’s a very common pattern that a lot of startups have today”) ^clm-1cb112ea83e55e1bd4db
- Altman says there have been four great platform shifts that let startups form at mass scale: the Internet, cloud, mobile, and AI. (§ AWS and Startups: “there was the Internet, there was cloud, there was mobile, and then there was AI”) ^clm-69763f8ad757efb0c121
- Altman says revenue at AI startups scales so fast that Y Combinator's expected revenue for a good company at the end of a batch changes every month. (§ AWS and Startups: “Well it’s kind of changing every month, maybe we’d have a different answer”) ^clm-31e6f23101b048c8fcee
- Altman says the harness (the software around the model: tools, memory, permissions) and the model are no longer separable, and he expects them to merge further over time, as tool-calling did. (§ Bedrock Managed Agents: “I no longer think of the harness and the model as these entirely separable things”) ^clm-d77c3cd156dba0207161
- Thompson argues the harness-model integration is the key integration point in the AI value chain, where value will collect; Altman agrees. (§ Bedrock Managed Agents: “my thesis then is that this harness-model integration is the key point”) ^clm-31db6aae9a5b31c75620
- Prediction: Altman predicts pre-training and post-training will also come together more over time. (§ Bedrock Managed Agents: “I would expect that pre-training and post-training eventually come together more over time”) ^clm-928a0b226eaf65a571dd
- Garman says that before this product, customers had to wire agents into their own data, tools, and systems on their own; the joint product builds in identity and keeps database access inside the customer's AWS VPC (a private network in AWS). (§ Bedrock Managed Agents: “the ability to go authenticate to your database all happens inside of your AWS VPC”) ^clm-54497147a8dd6eddd6d3
- Altman says Codex first ran in the cloud but moved to the user's local computer because it was easier to get working, though he expects agents to end up running in the cloud. (§ Local vs. Cloud: “Actually, we started with it running in the cloud, and I think eventually you do want it to run in the cloud”) ^clm-ce841691b528a47a63d9
- Altman says there is no basic building block yet for an agent logging in as a person while marking itself as an agent, and that access control and permission models will have to change as agents join the workforce. (§ Local vs. Cloud: “We don’t even have a primitive to think about that”) ^clm-5ca54a6802407aaeb7e1
- Garman says Bedrock Managed Agents was co-built by AWS and OpenAI teams from AgentCore components, AWS's existing set of agent building blocks (memory, safe execution, permissions). (§ AgentCore vs. Managed Agents: “The AWS team and the OpenAI team used AgentCore components together with the OpenAI models”) ^clm-28ac6921267337c607e9
- Altman says the managed agent offering is exclusive to Amazon, and says it is distinct from the plain API access OpenAI offers on Azure. (§ AgentCore vs. Managed Agents: “we’re doing this exclusively with Amazon, we’re excited about it”) ^clm-bd90d55e7500825f258f
- Garman says customer data stays inside the customer's VPC in the Bedrock environment. (§ AgentCore vs. Managed Agents: “the whole thing kind of stays within your VPC and so data is protected”) ^clm-0c5478aec058085ac7cf
- Prediction: Garman says the OpenAI models in Bedrock will run partly on Trainium (Amazon's own AI chip) and partly on GPUs, with more moving to Trainium over time. (§ AgentCore vs. Managed Agents: “But over time, more and more of it will be on Trainium”) ^clm-5743bddeb6ddab3e1294
- Garman argues most customers will reach AI chips only through abstractions like a model API, since most inference runs on a handful of models, so the chip underneath matters little to them. (§ Trainium: “the vast majority of inference out there is being done on one of a handful of models”) ^clm-6fddd7e98470cfa3ff53
- Altman says OpenAI's GPT-5.5 costs much more per token than 5.4 but needs far fewer tokens for the same answer, mostly due to the model, so per-token pricing may not last. (§ Trainium: “the per-token cost is much higher than 5.4, but it requires a hugely fewer number of tokens”) ^clm-0a16efd8f804cddec404
- Altman says OpenAI must be an intelligence factory, delivering the most units of intelligence at the lowest price, and customers do not care about the chip or model size underneath. (§ Trainium: “we’re like an intelligence factory or something”) ^clm-3769e62921b2f6f23f4d
- Garman says AWS will be frontline support for Bedrock Managed Agents and will escalate bugs to OpenAI when needed. (§ Customer Demand: “AWS will be that frontline support that you kind of interact with”) ^clm-fe9693c18c4047f76271
- Altman says OpenAI is committing to buy a lot of compute for this business and believes that at a low enough price, demand for intelligence is essentially uncapped. (§ Customer Demand: “at a low enough price, demand for intelligence is essentially uncapped”) ^clm-fd597abce89e68273b1a
- Altman says far more customers ask OpenAI for more capacity at any price than argue about price, and that so far most demand is for the absolute frontier (newest, best) models. (§ Customer Demand: “we have way more customers asking us, “No matter what the price is, can you give me more?”) ^clm-bdf289252b65063467d8
- Prediction: Garman predicts a mix of models over time: smaller, cheaper, faster ones alongside very large frontier ones. (§ Customer Demand: “I think over time, you will have a mix of models, by the way”) ^clm-174239575fb294c2d30e
- Altman says large enterprises now ask for a consistent package: an agent runtime, a management layer linking data to agents with token-spend oversight, and a workspace for employees. (§ Building the AI Stack: “that package of what people are asking for is getting remarkably consistent”) ^clm-31587b1e105588d16720
- Altman says ChatGPT is the first really large-scale new consumer product since Facebook, and that OpenAI has done better than he expected against Google, though he calls Google still underrated. (§ Building the AI Stack: “ChatGPT is, I think, the first really large-scale new consumer product since Facebook”) ^clm-304f2183b2c60e2fb611
- Garman says AWS's partner-first, model-neutral stance was partly deliberate, contrasting it with rivals like Google that try to own the whole stack from chip to agent. (§ Building the AI Stack: “Sometimes they say, “I have to own everything”, and that’s okay”) ^clm-e0e97bcf55c4530251b2

## Entities

[[AWS|AWS]], [[Amazon|Amazon]], [[Anthropic|Anthropic]], [[Google|Google]], [[Matt-Garman|Matt Garman]], [[Microsoft|Microsoft]], [[OpenAI|OpenAI]], [[Sam-Altman|Sam Altman]], Y Combinator

## Concepts

[[AI-Agents|AI Agents]], [[AI-Compute-Demand|AI Compute Demand vs Supply]], [[Conservation-of-Attractive-Profits|Conservation of Attractive Profits]], [[Custom-Silicon|Custom Silicon]]
