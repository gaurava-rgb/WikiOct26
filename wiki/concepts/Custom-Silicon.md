---
type: concept
title: Custom Silicon
status: developing
created: 2026-09-29
updated: 2026-09-29
tags:
  - concept
source_count: 14
card: true
---

# Custom Silicon

**In one sentence:** Custom silicon means chips a big company designs for its own needs instead of buying them from Nvidia, as Amazon, Meta, and Google began doing to beat the GPU shortage. ([[2025-Gallaugher-Ch08-Amazon|Gallaugher, Amazon, p.298]])

## Why it matters
Thompson argues that in a commodity market (where buyers only care about price), the cheapest supplier earns the most, so cheaper home-made chips mean bigger cloud profits. ([[2026-04-30-Amazon-Earnings-Trainium|Amazon earnings, Trainium]]) He also argues Anthropic and Google have shown Nvidia's software lock-in is not essential to train and run a leading model. ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia earnings, May]]) Gallaugher argues only the very largest firms have the money to design their own parts. ([[2025-Gallaugher-Ch08-Amazon|Gallaugher, Amazon, p.298]])

## Worked example: Amazon Trainium, early 2026
Amazon bought chip designer Annapurna Labs in 2015 to build chips like Trainium and Graviton. ([[2026-05-05-Amazons-Durability|Amazon's Durability]]) By early 2026 Trainium2 gave about 30% better price performance (work done per dollar) than comparable GPUs and was largely sold out. ([[2026-04-30-Amazon-Earnings-Trainium|Amazon earnings, Trainium]]) Amazon's chip business had a yearly revenue pace of over $20 billion, growing nearly 40% in one quarter. ([[2026-04-30-Amazon-Earnings-Trainium|Amazon earnings, Trainium]]) AWS held over $225 billion in promised Trainium spending, including from Anthropic and OpenAI. ([[2026-04-30-Amazon-Earnings-Trainium|Amazon earnings, Trainium]]) Andy Jassy expects Trainium to save Amazon tens of billions of dollars of capex (money spent on data centers and machines) each year. ([[2026-04-30-Amazon-Earnings-Trainium|Amazon earnings, Trainium]])

## Where analysts disagree
- In May 2026 all of OpenAI's work still ran on Nvidia chips ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia earnings, May]]). By August OpenAI had its own chip, and Huang argued OpenAI would stay a customer ([[2026-09-01-Nvidia-Earnings-Dollars-Per-Gigawatt-Open-and-Hugging-Face|Nvidia earnings, September]]). Thompson called that answer not compelling ([[2026-09-01-Nvidia-Earnings-Dollars-Per-Gigawatt-Open-and-Hugging-Face|Nvidia earnings, September]]).

## Used in
- [[stories/ai-shift-2024-2026|The AI shift, 2024 to 2026]]: the "chips go custom" chapter.
- [[journeys/amazon-journey|Amazon journey]]: Nitro, Graviton, and Trainium pay off.
- [[journeys/apple-journey|Apple journey]]: Apple Silicon drives the hardware bet.

## Sources
[[2025-Gallaugher-Ch08-Amazon|Gallaugher, Amazon]] · [[2026-04-20-TSMC-Earnings-New-N3-Fabs-The-Nvidia-Ramp|TSMC earnings]] · [[2026-04-22-John-Ternus-and-Apples-Hardware-Defined-Future-SpaceXAI-and-Cursor|Ternus and SpaceXAI]] · [[2026-04-23-Interview-Thomas-Kurian-Google-Cloud|Kurian interview]] · [[2026-04-28-Interview-Altman-Garman-Bedrock-Managed-Agents|Altman and Garman interview]] · [[2026-04-29-Intel-Earnings-Intels-Differentiation-Whither-Terafab|Intel earnings]] · [[2026-04-30-Amazon-Earnings-Trainium|Amazon earnings, Trainium]] · [[2026-05-04-Google-Earnings-Meta-Earnings|Google and Meta earnings]] · [[2026-05-05-Amazons-Durability|Amazon's Durability]] · [[2026-05-06-Microsoft-Earnings-Apple-Earnings|Microsoft and Apple earnings]] · [[2026-05-14-Interview-Ben-Thompson-MoffettNathanson|MoffettNathanson interview]] · [[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia earnings, May]] · [[2026-06-02-The-Google-Capital-Company|The Google Capital Company]] · [[2026-09-01-Nvidia-Earnings-Dollars-Per-Gigawatt-Open-and-Hugging-Face|Nvidia earnings, September]]

## Change log
- 2026-09-29: first build from proposal 2026-09-29.

<!-- claims: clm-115a00f7f523e8b21978, clm-419617325d8f6b2675f2, clm-c40b6055bf2baa89bccb, clm-9fa8a432ceca0f27f666, clm-e629fa6598d732768f7c, clm-1b982aadfe863ef4891b, clm-bdf83c9776a9958879c8, clm-19581e27de7ced00ff1c, clm-87b4d9d1be3c62f5ca44, clm-b77c656a72328b241648, clm-a38c8566269d8bd2f5a0, clm-2688c7fb192c10387f14 -->
