---
type: source
title: Frontier Overhangs
status: evergreen
created: 2026-09-29
updated: 2026-09-29
tags:
  - source
  - source/article
author: Ben Thompson
published: 2026-09-21
publisher: Stratechery
url: "https://stratechery.com/2026/frontier-overhangs/"
raw: .raw/captured/Frontier Overhangs.md
source_id: src-d1ee4c82069df2fa1b8a
---

# Frontier Overhangs

Ben Thompson, Stratechery, published 2026-09-21.

## Summary

Thompson looks at Dario Amodei's call to pace the frontier of AI and asks what it does for the business of the top labs. He names four overhangs, gaps built up because models got better so fast: capability, product, pricing, and capital. Slowing down would give Anthropic and OpenAI time to build sticky products, sell their compute for use instead of training, and let revenue catch up with spending. On safety, he argues that pacing actually hurts, because defenders still need better models to fight automated hackers. He ends by saying the real overhang is competition, since the call to slow down came just as OpenAI took the lead.

## Key claims

- Thompson argues that Anthropic's call to pace the frontier is sincerely about safety but also happens to solve several business problems for the frontier labs. (“it also happens to address several distinct problems faced by the frontier labs”) ^clm-b80150b0f6b17aabe08d
- Thompson argues these problems are overhangs formed because models improve so fast, and slowing model progress would shrink them. (“slowing model improvement would reduce the overhangs”) ^clm-248778092a14053eaa3d
- Thompson dates the agentic paradigm to the release of Opus 4.5 in late November 2025, and says it is so token hungry that AI infrastructure is not a bubble. (§ The Capability Overhang: “kicked off with the release of Opus 4.5 in late November 2025”) ^clm-a6f46b4de3c3a3ac749e
- Satya Nadella said Microsoft uses one multi-model harness across GitHub and security, with MAI by default plus GPT, Anthropic, and open weight models. (§ The Capability Overhang: “we have the same harness that's a multi-model harness in which we will rotate through”) ^clm-bdf5d8e715d955ae72eb
- Users can now choose which model runs Copilot Cowork, which Thompson says shows the harness and the model can be separate things. (§ The Capability Overhang: “clearly the harness and the model can be different things”) ^clm-9d64ea7f97d02e071886
- Thompson has wavered on his earlier view that model and harness integration is where agent differentiation lies. (§ The Capability Overhang: “one part of that Article that I've wavered on, and that is the importance of model company harnesses”) ^clm-976470588c13781bc6d3
- Anthropic had made Fable use depend on keeping all customer data for at least a month, but customers pushed back and Fable usage stayed relatively low. (§ The Capability Overhang: “Fable wasn't good enough: customers pushed back, and Fable usage stayed relatively low”) ^clm-0bde8d4379302c37ea95
- When Fable 5.1 was released, Anthropic dropped the rule that let it keep customer data. (§ The Capability Overhang: “when Fable 5.1 was released, the Anthropic-gets-to-keep-your-data provision was gone”) ^clm-6d11785bc5cc78e3d4cb
- Thompson argues the Fable episode shows Christensen's theory at work: current models are good enough that customers weigh data policy over pure performance, so pure capability is no longer a moat. (§ The Capability Overhang: “Pure capability no longer translates directly into a moat”) ^clm-406c6b82d3479c0b0079
- Thompson argues frontier labs have an economic need to own the user touchpoint and replace software, and must build those touchpoints while they still have better capabilities. (§ The Product Overhang: “build those user touchpoints while they have superior capabilities”) ^clm-48f47275125759deaf63
- Thompson calls Meta's Muse the best and most approachable personal agent product he has tried, running on a free, capable virtual machine. (§ The Product Overhang: “the best and most approachable personal agent product I have tried”) ^clm-3b24ab3b27e53bf5d04b
- Thompson sees Muse as a bearish sign for the frontier labs: Muse Spark 1.3 is not state of the art yet is good enough for a very sticky personal agent. (§ The Product Overhang: “Muse Spark 1.3, the most advanced Meta model, is still not state-of-the-art”) ^clm-54549760b1f716c150d1
- Thompson argues coding agents have little lock-in because the code lives in GitHub, so switching to another agent and harness is easy. (§ The Product Overhang: “it's not that much of a lift to point a different agent and harness”) ^clm-15f5484c832521c85cf9
- Thompson argues Anthropic and OpenAI would do well to spend more of their resources building products with real moats. (§ The Product Overhang: “it would do Anthropic and OpenAI good to devote more of their resources to actually building such products”) ^clm-e3d064784ca41654f23a
- Thompson argues Chinese models only look cheaper because Anthropic and OpenAI are supply constrained and charge a price umbrella above what full supply would allow. (§ The Pricing Overhang: “Right now there is a price umbrella that is downstream of the lack of compute”) ^clm-02321f8333e8a34c126e
- Thompson argues that if the labs slowed progress they could move compute from training and research to inference and fully capture the market. (§ The Pricing Overhang: “If they slowed down progress they could re-allocate computing and fully capture the market”) ^clm-ba522d3d3e7ea1989774
- Per the Financial Times, Anthropic told backers its adjusted operating income would be positive for a second straight quarter, ahead of a planned IPO. (§ The Capital Overhang: “its adjusted operating income will be positive for the second consecutive quarter”) ^clm-e7658eb251b288e3ef37
- Per the Financial Times, Anthropic's gross margins are above 80 per cent before revenue shared with partners such as Amazon and before training costs. (§ The Capital Overhang: “Anthropic's gross margins are above 80 per cent before accounting for revenue shared with distribution partners”) ^clm-83f3a0f05d74c9ba9e7a
- Thompson added a correction saying he was told Anthropic is profitable even including training costs. (§ The Capital Overhang: “I am told that Anthropic is indeed profitable including training costs”) ^clm-c5c11119d9a23c9067bf
- Prediction: Thompson argues the labs, hyperscalers, and neoclouds all need AI revenue to rise sharply, since capital is limited and hitting that limit would end badly for anyone relying on outside funding. (§ The Capital Overhang: “there is a limit to available capital, and finding that limit will end badly”) ^clm-12969bf412e580c59cd9
- Thompson argues AI cyberattacks favor attackers, since automated attacks always have positive expected value while automated defense has negative expected value. (§ The Safety Overhang: “The expected value for a hacker's automated attack is always positive”) ^clm-8523a1f8ad31c170649f
- Thompson argues cyber risk is not alignment risk, and that there is no evidence of LLMs having a will or acting with malice. (§ The Safety Overhang: “there simply isn't any evidence of LLMs having a will or operating with malevolence”) ^clm-d4224f49dd97f3cb2118
- Thompson argues that pacing the frontier makes today's real safety risk worse, because defenders need better models to automate defense. (§ The Safety Overhang: “pacing the frontier actually increases the window in which bad things can happen”) ^clm-e3b6c29de871f5f1a6d6
- Thompson notes the call to pace the frontier came when OpenAI, for the first time in a while, held the lead, and says Anthropic exists because its founders distrusted Sam Altman. (§ The Safety Overhang: “the demand to pace the frontier came when the frontier was, for the first time in a while, set by OpenAI”) ^clm-dbebc729b27184fb1dc2
- Thompson argues the overhang that matters most is competition: Anthropic is fine being in the lead, but anyone else leading requires government action. (§ The Safety Overhang: “that's probably the overhang that matters most of all: competition”) ^clm-7a90fe3cb28c8c72f4b4

## Entities

[[Amazon|Amazon]], [[Anthropic|Anthropic]], [[Clayton-Christensen|Clayton Christensen]], [[Dario-Amodei|Dario Amodei]], [[Google|Google]], [[Meta|Meta]], [[Microsoft|Microsoft]], [[Nvidia|Nvidia]], [[OpenAI|OpenAI]], [[Sam-Altman|Sam Altman]], [[Satya-Nadella|Satya Nadella]]

## Concepts

[[AI-Agents|AI Agents]], [[AI-Compute-Demand|AI Compute Demand vs Supply]], [[Commodity-Cost-Advantage|Winning a Commodity Market on Cost]], [[Conservation-of-Attractive-Profits|Conservation of Attractive Profits]], Price Umbrella (Price Overhang)
