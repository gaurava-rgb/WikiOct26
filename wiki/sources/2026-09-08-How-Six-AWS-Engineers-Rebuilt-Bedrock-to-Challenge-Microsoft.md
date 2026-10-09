---
type: source
title: How Six AWS Engineers Rebuilt Bedrock to Challenge Microsoft
status: evergreen
created: 2026-10-08
updated: 2026-10-08
tags:
  - source
  - source/article
author: Catherine Perloff and Kevin McLaughlin
published: 2026-09-08
publisher: The Information
url: "https://www.theinformation.com/articles/six-aws-engineers-rebuilt-bedrock-challenge-microsoft"
raw: .raw/captured/2026-09-08 The Information - Six AWS engineers rebuilt Bedrock to challenge Microsoft (notes).md
source_id: src-ddeb029b8cdae1385107
---

# How Six AWS Engineers Rebuilt Bedrock to Challenge Microsoft

Catherine Perloff and Kevin McLaughlin, The Information, published 2026-09-08.

## Summary

AWS's Bedrock AI model service was rushed out in 2023 and by early 2025 was buggy, throttled and slow, with customers waiting up to three weeks for capacity. Six senior engineers rebuilt it as Project Mantle, launched December 2025, treating inference as a scheduling problem rather than a web service and adding priorities, customer isolation and agent support. Capacity waits fell to two days, Bedrock moved mostly onto Trainium chips, and AWS added OpenAI models. Bedrock usage surged in 2026 and AWS growth sped to 37%, with consultants saying AWS is pulling spending from Azure.

## Key claims

- In early 2025 AWS's Bedrock service was buggy, with repeated error messages and waits of weeks for computing capacity, per people with knowledge. (§ The core story: “Customers saw repeated error messages and sometimes waited weeks for computing capacity”) ^clm-dfcbc1f532f17d5b88bb
- Senior AWS engineer Anthony Liguori and five other senior engineers designed a rebuilt Bedrock called Project Mantle to fix throttling and errors and let it scale. (§ The core story: “Anthony Liguori and five other senior engineers designed a rebuilt version called”) ^clm-f37b63a5fc4e580ef4d1
- The Mantle team built it using Kiro, AWS's in-house AI coding tool. (§ The core story: “They built it using Kiro, AWS's in-house AI coding tool”) ^clm-d1098d8ef919e4b9eef7
- Mantle launched in December 2025, and a few months later AWS added OpenAI models to Bedrock. (§ The core story: “Mantle launched in December 2025. A few months later AWS added OpenAI models to Bedrock”) ^clm-73b3319edbfd51354e88
- Randall Hunt, CTO of AWS consultancy Caylent, says AWS is now pulling some spending away from Microsoft Azure, and his financial services clients' AWS spending grew five times since May. (§ Results: “AWS is now pulling some spending away from Microsoft Azure”) ^clm-ac960ae0e543a268907c
- Amazon said it added more Bedrock customers in the first half of 2026 than in the service's first two years, and Q2 Bedrock spending beat all prior quarters combined. (§ Results: “Q2 Bedrock spending beat all prior quarters combined”) ^clm-f1d1dce10defec306f52
- AWS growth sped up 9 percentage points to 37% in Q2 2026, while Azure grew 42%. (§ Results: “AWS growth sped up 9 percentage points to 37% in Q2”) ^clm-4e90e336161467bf40ed
- Bedrock launched in fall 2023 in a rush after ChatGPT caught Amazon off guard, and later staff said the build felt glued together and did not fully use its chip capacity. (§ How Bedrock got into trouble: “The rushed build felt "glued together"”) ^clm-470f7d3676511e5f0209
- Customers complained throughout 2025 about throttled access to Anthropic models on Bedrock, and AWS leaders worried coding startup Lovable might leave. (§ How Bedrock got into trouble: “Customers complained all through 2025 about throttled access to Anthropic models”) ^clm-308db1e6ca3053a224ea
- Hunt says in 2024 his clients found Anthropic models ran up to 63% slower on Bedrock, in tokens per second, than on Anthropic's own API. (§ How Bedrock got into trouble: “Anthropic ran up to 63% slower on Bedrock”) ^clm-6d88e75185981b705f91
- Former AWS VP Joe Magerramov, who helped build Mantle, argued that inference is closer to a scheduling system than a web service. (§ What Mantle changed: “inference is closer to a scheduling system than a web service”) ^clm-441c5da57957993cbf57
- Mantle handles spiky workloads, lets customers set task priorities, isolates customers from each other, and works with AWS Journal, which saves an agent's progress so long tasks need not restart. (§ What Mantle changed: “saves an AI agent's progress so long tasks need not restart after a failure”) ^clm-27d78d57dd5fcdc31647
- The wait for extra Bedrock capacity fell from three weeks to two days by late 2025, per a former employee. (§ What Mantle changed: “Wait for extra capacity fell from three weeks to two days by late 2025”) ^clm-8f20f49d4011543d309f
- Later in 2025 Bedrock moved to running mostly on Amazon's own Trainium chips, easing reliance on scarce Nvidia chips. (§ What Mantle changed: “Bedrock moved to running mostly on Amazon's own Trainium AI chips”) ^clm-f44d80174e82b0898932
- Mantle leaders Dave Brown and Joe Magerramov have left AWS for Meta. (§ What Mantle changed: “He followed Brown to Meta last month”) ^clm-a8693da4b6ab4a89448f

## Entities

[[AWS|AWS]], [[Amazon-Bedrock|Amazon Bedrock]], Anthony Liguori, [[Anthropic|Anthropic]], [[Meta|Meta]], [[Microsoft|Microsoft]], [[Nvidia|Nvidia]], [[OpenAI|OpenAI]], [[Randall-Hunt|Randall Hunt]], [[Trainium|Trainium]]

## Concepts

[[AI-Agents|AI Agents]], [[Custom-Silicon|Custom Silicon]]
