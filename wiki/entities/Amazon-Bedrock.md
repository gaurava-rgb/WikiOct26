---
type: entity
title: Amazon Bedrock
status: developing
created: 2026-10-08
updated: 2026-10-21
tags:
  - entity
  - entity/product
claim_count: 11
---

# Amazon Bedrock

AWS service that lets customers run AI models such as Claude and OpenAI models inside Amazon's cloud; launched 2023.

## Facts by source

### 2026-09-08 [[2026-09-08-How-Six-AWS-Engineers-Rebuilt-Bedrock-to-Challenge-Microsoft|How Six AWS Engineers Rebuilt Bedrock to Challenge Microsoft]]

- In early 2025 AWS's Bedrock service was buggy, with repeated error messages and waits of weeks for computing capacity, per people with knowledge. ([[2026-09-08-How-Six-AWS-Engineers-Rebuilt-Bedrock-to-Challenge-Microsoft#^clm-dfcbc1f532f17d5b88bb|cite]])
- Senior AWS engineer Anthony Liguori and five other senior engineers designed a rebuilt Bedrock called Project Mantle to fix throttling and errors and let it scale. ([[2026-09-08-How-Six-AWS-Engineers-Rebuilt-Bedrock-to-Challenge-Microsoft#^clm-f37b63a5fc4e580ef4d1|cite]])
- Mantle launched in December 2025, and a few months later AWS added OpenAI models to Bedrock. ([[2026-09-08-How-Six-AWS-Engineers-Rebuilt-Bedrock-to-Challenge-Microsoft#^clm-73b3319edbfd51354e88|cite]])
- Amazon said it added more Bedrock customers in the first half of 2026 than in the service's first two years, and Q2 Bedrock spending beat all prior quarters combined. ([[2026-09-08-How-Six-AWS-Engineers-Rebuilt-Bedrock-to-Challenge-Microsoft#^clm-f1d1dce10defec306f52|cite]])
- Bedrock launched in fall 2023 in a rush after ChatGPT caught Amazon off guard, and later staff said the build felt glued together and did not fully use its chip capacity. ([[2026-09-08-How-Six-AWS-Engineers-Rebuilt-Bedrock-to-Challenge-Microsoft#^clm-470f7d3676511e5f0209|cite]])
- Customers complained throughout 2025 about throttled access to Anthropic models on Bedrock, and AWS leaders worried coding startup Lovable might leave. ([[2026-09-08-How-Six-AWS-Engineers-Rebuilt-Bedrock-to-Challenge-Microsoft#^clm-308db1e6ca3053a224ea|cite]])
- Hunt says in 2024 his clients found Anthropic models ran up to 63% slower on Bedrock, in tokens per second, than on Anthropic's own API. ([[2026-09-08-How-Six-AWS-Engineers-Rebuilt-Bedrock-to-Challenge-Microsoft#^clm-6d88e75185981b705f91|cite]])
- Former AWS VP Joe Magerramov, who helped build Mantle, argued that inference is closer to a scheduling system than a web service. ([[2026-09-08-How-Six-AWS-Engineers-Rebuilt-Bedrock-to-Challenge-Microsoft#^clm-441c5da57957993cbf57|cite]])
- Mantle handles spiky workloads, lets customers set task priorities, isolates customers from each other, and works with AWS Journal, which saves an agent's progress so long tasks need not restart. ([[2026-09-08-How-Six-AWS-Engineers-Rebuilt-Bedrock-to-Challenge-Microsoft#^clm-27d78d57dd5fcdc31647|cite]])
- The wait for extra Bedrock capacity fell from three weeks to two days by late 2025, per a former employee. ([[2026-09-08-How-Six-AWS-Engineers-Rebuilt-Bedrock-to-Challenge-Microsoft#^clm-8f20f49d4011543d309f|cite]])
- Later in 2025 Bedrock moved to running mostly on Amazon's own Trainium chips, easing reliance on scarce Nvidia chips. ([[2026-09-08-How-Six-AWS-Engineers-Rebuilt-Bedrock-to-Challenge-Microsoft#^clm-f44d80174e82b0898932|cite]])

## Related concepts

[[AI-Agents|AI Agents]], [[Custom-Silicon|Custom Silicon]]
