---
type: source
title: An Interview with Google Cloud CEO Thomas Kurian About the Agentic Moment
status: evergreen
created: 2026-09-29
updated: 2026-09-29
tags:
  - source
  - source/interview
author: Ben Thompson
published: 2026-04-23
publisher: Stratechery
url: "https://stratechery.com/2026/an-interview-with-google-cloud-ceo-thomas-kurian-about-the-agentic-moment/"
raw: .raw/captured/An Interview with Google Cloud CEO Thomas Kurian About the Agentic Moment.md
source_id: src-6439957cd04601c9b8fc
---

# An Interview with Google Cloud CEO Thomas Kurian About the Agentic Moment

Ben Thompson, Stratechery, published 2026-04-23.

## Summary

Ben Thompson talks with Google Cloud CEO Thomas Kurian ahead of Google Cloud Next 2026. Kurian says customers have moved from chatbots to agents that run whole business processes, and that Google wins because it owns every layer: chips, models, data tools, security, and the agent platform. He shares growth numbers for Gemini, new TPU chips, a plan to put TPUs in other companies' data centers, and why selling compute to rivals like Anthropic is not a loss. It matters because it shows how Google plans to turn its full AI stack into a cloud business.

## Key claims

- Kurian says the framing for Google Cloud Next 2026 is that customers are moving from using AI to answer questions like a chatbot to having it automate tasks and whole process flows. (§ Agents: “evolving the use of AI models from being used to answer questions in a chatbot-like fashion”) ^clm-e2d19bdafd9089e7231f
- Kurian says agents got much better in the past year because models reason better, keep long-running memory, and use tools through standard abstractions like skills and MCP. (§ Agents: “they’re able to maintain long-running memory, which you require if you have an agent”) ^clm-9ca6435e3992477dc7d7
- Thompson notes that Gemini was the hot model around the end of 2025, but talk has since shifted mostly to Anthropic's Claude and OpenAI's Codex. (§ Agents: “Gemini was the belle of the ball four months ago”) ^clm-243201859c5b98438bea
- Kurian says about 500 customers, including Citigroup, Comcast, Walmart, and Unilever, would tell their agent stories at Next. (§ Agents: “you’re going to hear from 500 customers telling their stories at Next”) ^clm-36811c2697191eb7e8ed
- Kurian argues that business processes with many constraints need smarter models, not simpler ones, because there are too many odd cases to program ahead of time, so the model must write code to handle them. (§ Agents: “having constraints requires the model to be even more intelligent”) ^clm-c75ef9f9a2138e452240
- Kurian says customer workflows from Google Cloud are put into a harness that feeds the reinforcement (training) loop for Gemini, with Cloud staff sitting next to Demis Hassabis's DeepMind team. (§ Integrating With Google: “we put them into the harness and they get into the reinforcement loop for Gemini”) ^clm-4a09a0efbb5a100e2248
- Kurian argues Google is unique in AI because it owns the whole stack, and says that stack improves the models 'literally every hour of every day'. (§ Integrating With Google: “we’re unique because we have the whole stack of AI technology”) ^clm-e395ebd23b95d977ed81
- Kurian says every Google product runs on the same Gemini version and the same agent harness at the same time. (§ Integrating With Google: “Every product that Google has is on the same Gemini version, on the same day”) ^clm-a5c379e0735e59ceda0a
- Google generates 16 billion tokens a minute, up from 10 billion around December 2025 or January 2026. (§ Integrating With Google: “we generate 16 billion tokens a minute, up from 10 just last December or January”) ^clm-5a77726754ab2b2fcf05
- Kurian says Gemini tokens grew 40% since the prior quarter and Gemini Enterprise, Google's core agent platform, grew 40% quarter over quarter. (§ Cloud Priorities: “has grown 40% sequentially quarter-over-quarter”) ^clm-70180926a8a80d1ecc6e
- Kurian says most of the large AI labs, including Anthropic, use Google's stack, and Google makes money from whichever layer they buy, such as TPUs, Gemini, or security, so it does not see this as zero sum. (§ Cloud Priorities: “most of the large AI labs use our stack”) ^clm-ce3b89243008384860dd
- Kurian argues selling TPUs to outsiders fills idle chips at night when chat demand drops, and the higher volume gets better supplier terms, which lowers cost of goods sold (the direct cost of what Google sells). (§ Cloud Priorities: “that in turn lowers our cost of goods sold”) ^clm-8dd38ead112a81582a5c
- Google announced TPU 8t for training, a pod of 9,600 chips with three times the performance of the current generation. (§ Cloud Priorities: “think of it as 9,600 TPU chips, a single pod”) ^clm-454e87fc20e0c656f0e3
- Google announced TPU 8i for inference (running models), with 1,152 chips, three times the SRAM (fast on-chip memory), and a new Collectives Engine. (§ Cloud Priorities: “it’s 1,152 chips, three times the SRAM”) ^clm-1c687a52b72ab9a10d1d
- Google Cloud also announced Nvidia VR200 instances, more ARM computers for classical tasks, a 10 terabit-per-second Lustre storage product, and a low-latency Rapid Storage product. (§ Cloud Priorities: “we are introducing Nvidia VR200, we’re also introducing more ARM capability for classical compute”) ^clm-4a4af3dee2be5b50cbf9
- Kurian says new TPU buyers include capital markets firms like Citadel Securities that want to replace algorithmic trading on x86 chips, and high performance computing users like the Department of Energy's Genesis mission. (§ Cloud Priorities: “a big new segment is financial services and when I say financial services, capital markets”) ^clm-0899fd794565259f747c
- Google will put TPUs in other companies' own sites and sell them as a system, not only as cloud rental, for customers like trading firms and national labs. (§ Cloud Priorities: “you will see us putting TPU in other people’s venues”) ^clm-ee542fdfc04b5ff8358a
- Kurian says the TPUs in third-party data centers are identical to cloud TPUs and come from Google's global allocation, made with partner Broadcom. (§ Cloud Priorities: “Broadcom partner who manufactures the TPUs with us”) ^clm-e3d73003187deb217907
- Kurian says compute is always short, even though Google could not grow as fast as it does without enough of it. (§ Cloud Priorities: “there’s always a shortage, there’s never enough”) ^clm-a7eb6e8057f126a37430
- Kurian says Google Cloud splits its business into Gemini as a product, Gemini embedded in other products, and selling compute, and argues placing hardware in customer sites changes cash flow compared with spending its own capex (money on data centers). (§ Cloud Priorities: “we drive cash flow in a different way than putting CapEx”) ^clm-7d8d877aa2ff3015b6cd
- Kurian's team builds all the infrastructure for Alphabet and also runs the cloud business, and he calls the idea that giving compute to one side takes from another overly simplistic. (§ Cloud Priorities: “We are responsible for delivering all the infrastructure for Alphabet”) ^clm-22f9a23809101cc510de
- Kurian says Gemini in Google's threat intelligence tools is 98% accurate at ranking threats and processed 3.9 million threats in the last year. (§ Cloud Priorities: “it’s 98% accurate and has processed 3.9 million threats in the last year”) ^clm-aadd804e10695c22bcb1
- Kurian says Google bought Wiz because AI will find software holes much faster, so customers must fix them much faster, and cloud is the most valuable place to protect. (§ Cybersecurity: “we said to ensure that we have the leading product portfolio, let’s acquire Wiz”) ^clm-e32ac02bb9849f3bacb6
- Google and Wiz launched three Gemini agents: Red Agent tests attacks, Blue Agent finds what to fix, and Green Agent fixes it. (§ Cybersecurity: “one called Red Agent — think of it as continuous red-teaming of your infrastructure”) ^clm-69f4c9640e73e136870e
- Thompson argues the Wiz deal answers why Google bought instead of built: in two years building would have been too late. (§ Cybersecurity: “in two years, it’s going to be too late”) ^clm-3b4878b9b30d64259a6b
- Google's cross-cloud lakehouse lets customers query data left in AWS, Azure, and SaaS apps, avoiding the egress fees (charges to move data out) other clouds impose, and Kurian claims 2x better price performance than the market leader. (§ Knowledge Graph: “we’re 2x better in price performance than the market leader”) ^clm-5f0a092fcf9b6b2c54aa
- Kurian says Knowledge Catalog uses Gemini, not human consultants, to build a map of what each company's data means, and says Google is not competing with Palantir's ontology. (§ Knowledge Graph: “we use Gemini, so we don’t need humans”) ^clm-0bc4d31bd9e07aa97814
- Kurian says Google would love to offer OpenAI models on Vertex, and is adding third-party models including Anthropic and open source ones. (§ Models and Partners: “We would love to have them”) ^clm-37a06c8b86bca54338e9
- Kurian rejects Thompson's idea that the model will eat all software, saying many SaaS vendors are embedding Gemini as an agent platform and Google will invest to grow its partner ecosystem. (§ Models and Partners: “we definitely don’t see that all the ecosystem is going to die”) ^clm-dfa422f63505c65bb16c
- Kurian claims Google is the only company with chips, models, data context, cyber tools, and a world-class agent platform. (§ Models and Partners: “We’re the only ones with chips, models, the context to feed the models”) ^clm-b8e3d3fa3dca974631bb
- Sundar Pichai said at the Next keynote that half of Google's capex (spending on data centers) goes to Google Cloud, which runs the same stack as Google itself. (“half of it was going towards Google Cloud”) ^clm-84614cc34ce7f2617249

## Entities

[[AWS|AWS]], [[Anthropic|Anthropic]], [[Ben-Thompson|Ben Thompson]], [[Broadcom|Broadcom]], [[Google|Google]], [[Google-Cloud|Google Cloud]], Google DeepMind, [[Microsoft|Microsoft]], [[Nvidia|Nvidia]], [[OpenAI|OpenAI]], Sundar Pichai, [[Thomas-Kurian|Thomas Kurian]], [[Wiz|Wiz]]

## Concepts

[[AI-Agents|AI Agents]], [[AI-Compute-Demand|AI Compute Demand vs Supply]], Full-Stack AI Integration, [[Aggregation-Theory|Aggregation Theory]], [[Commodity-Cost-Advantage|Winning a Commodity Market on Cost]], [[Custom-Silicon|Custom Silicon]]
