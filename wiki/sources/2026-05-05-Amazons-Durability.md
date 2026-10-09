---
type: source
title: Amazon’s Durability
status: evergreen
created: 2026-09-29
updated: 2026-09-29
tags:
  - source
  - source/article
author: Ben Thompson
published: 2026-05-05
publisher: Stratechery
url: "https://stratechery.com/2026/amazons-durability/"
raw: .raw/captured/Amazon’s Durability.md
source_id: src-1868d7761fd537d6f59f
---

# Amazon’s Durability

Ben Thompson, Stratechery, published 2026-05-05.

## Summary

Amazon Supply Chain Services fulfills Thompson's 2016 'Amazon Tax' prediction that Amazon would sell its logistics like AWS. He retells how AWS won a commodity market on cost (Nitro, Graviton), why it looked behind in the 2023 training era, and why the shift to inference and agents favors its chips, networking, and neutrality. Leo satellites may be the next long bet. He links a company's AI incentives to how physical its business is.

## Key claims

- Amazon unveiled Amazon Supply Chain Services (ASCS) bundling its freight and distribution offerings. (“announced Amazon Supply Chain Services (ASCS)”) ^clm-3fdba35f04dc8c462986
- Procter & Gamble and 3M are using Amazon's Supply Chain Services. (“companies like Procter & Gamble Co. and 3M Co. are already using”) ^clm-8527a891e224136950ff
- Amazon bought Annapurna Labs in 2015 to build custom chips like Trainium and Graviton. (§ Training vs. Inference: “Amazon bought Annapurna Labs, which makes their chips, in 2015”) ^clm-e629fa6598d732768f7c
- Amazon Supply Chain Services packages air and ocean freight, trucking, and last-mile delivery for other companies, and sent FedEx and UPS shares lower. (“sending shares of rival delivery companies such as FedEx Corp. and United Parcel Service Inc. lower”) ^clm-9af9229107d6d938e48d
- Thompson says ASCS fulfills his 2016 'The Amazon Tax' prediction that Amazon would sell its logistics network to third parties, the same way it sells AWS. (“the culmination of a prediction I made a decade ago in The Amazon Tax”) ^clm-c3f9f5f964575520904f
- In 2016 Amazon had experimented with six planes and leased 20 more to build a private logistics network. (“after experimenting with six planes last year the company recently leased 20 more”) ^clm-42e4175e56e99f8a5305
- Thompson argues Amazon works on decade-long timeframes, converting marginal costs into capital costs and then selling that capacity to other businesses. (“convert their marginal costs into capital costs and (2) gain leverage on those capital costs”) ^clm-7cbe960648324f6453cd
- Amazon invented cloud computing and realized it would be a commodity market where profit comes from structurally cheaper costs. (§ A Brief History of AWS: “Amazon not only invented cloud computing, but also realized it would be a commodity market”) ^clm-4405974051ccc206e49a
- AWS's Nitro system, built on its own chips, offloaded server management from Intel and AMD servers so each server could run more virtual machines. (§ A Brief History of AWS: “AWS built a specialized system called Nitro, built on their own chips”) ^clm-293d4819c0dcd6be8e36
- Early Graviton ARM chips were inferior to Intel and AMD chips but still paid off by quietly powering platform services like RDS. (§ A Brief History of AWS: “Graviton chips, particularly the first few generations, were inferior to Intel or AMD chips”) ^clm-da17640aec2771bad40c
- SemiAnalysis argued in 2023 that AWS would lose the future of computing because it used its own networking instead of Nvidia's or Broadcom's and got fewer Nvidia GPUs. (§ Training vs. Inference: “Rather than implement the best networking from Nvidia and/or Broadcom, Amazon is using its own Nitro”) ^clm-e8df189f2fe337c1a7db
- Thompson says training, which needs large networked GPU clusters, is no longer the biggest AI compute market; inference is. (§ Training vs. Inference: “training is no longer the biggest AI compute market; inference is”) ^clm-2cae7ea16f4786556fe6
- Thompson argues inference and agents favor AWS: models fit in one server, agent memory needs dedicated memory servers, and agents are CPU heavy. (§ Training vs. Inference: “Both the shift to inference and the shift in the nature of inference have been positives for AWS’ approach”) ^clm-5781e16870e34e6c08fd
- Jensen Huang argued at GTC 2025 that AI factories are power constrained, so tokens-per-watt matters more than chip cost; Thompson gives three reasons this may not hold for Amazon. (§ Training vs. Inference: “the most important metric for profitability was not the cost of chips but rather tokens-per-watt”) ^clm-f505cbe2522b26c3a2f3
- Amazon launched its first AI-focused chip in 2019; Thompson calls Trainium 3 decent with an even better trajectory. (§ Training vs. Inference: “launched their first AI-focused chip in 2019”) ^clm-5c9e54d4089facc33dd9
- Jensen Huang said Nvidia's mistake was not investing in Anthropic early, when Google and AWS made huge investments so Anthropic would use their compute. (§ AWS’s Neutrality: “We just weren’t in a position to make the multi-billion dollar investment into Anthropic”) ^clm-c2d2d8d18f3f81d8aa1e
- Anthropic was for a long time the only frontier model available on all the leading clouds, a selling point for enterprises. (§ AWS’s Neutrality: “for a long time was the only frontier model available on all of the leading clouds”) ^clm-0f296fecff83ca20f589
- Microsoft missed Azure growth projections earlier in 2026 because it gave more compute to internal AI workloads. (§ AWS’s Neutrality: “the company missed Azure growth projections because they devoted more compute to their internal workloads”) ^clm-0c56c9e75500d7cfd9ee
- Andy Jassy said Amazon Leo has over 20 launches planned in 2026 and over 30 in 2027, and could be a many-billion-dollar business with AWS-like economics. (§ Amazon’s Future: “We have over 20 launches planned this year. We have over 30 launches planned in 2027”) ^clm-249e7fd5715485171fa8
- Prediction: Thompson speculates Leo could support drone delivery so Amazon does not depend on Elon Musk for connectivity. (§ Amazon’s Future: “do you think they want to be dependent on Elon Musk for drone connectivity”) ^clm-33b8815695e84717f474
- Thompson argues a company's incentive to invest in AI tracks how little it touches the physical world: Apple and Amazon are fine with model access, while aggregators Google and Meta need their own models. (§ Amazon’s Future: “Apple and Amazon feel comfortable not having leading edge models, just access to them”) ^clm-8dec3a4bd9fc28d0e060

## Entities

3M, [[AMD|AMD]], [[AWS|AWS]], [[Amazon|Amazon]], [[Andy-Jassy|Andy Jassy]], Annapurna Labs, [[Anthropic|Anthropic]], [[Apple|Apple]], Broadcom, Elon Musk, FedEx, [[Google|Google]], [[Intel|Intel]], [[Jensen-Huang|Jensen Huang]], [[Meta|Meta]], [[Microsoft|Microsoft]], [[Nvidia|Nvidia]], Procter & Gamble, [[SpaceX|SpaceX]], UPS

## Concepts

[[AI-Agents|AI Agents]], [[AI-Compute-Demand|AI Compute Demand vs Supply]], [[Aggregation-Theory|Aggregation Theory]], [[Commodity-Cost-Advantage|Winning a Commodity Market on Cost]], [[Custom-Silicon|Custom Silicon]], First and Best Customer (Amazon Primitives), [[LLM-Inflection-Points|Three LLM Inflection Points]]
