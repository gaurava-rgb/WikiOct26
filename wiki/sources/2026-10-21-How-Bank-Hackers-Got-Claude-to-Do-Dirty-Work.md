---
type: source
title: How Bank Hackers Got Claude to Do Their Dirty Work
status: evergreen
created: 2026-10-21
updated: 2026-10-21
tags:
  - source
  - source/article
author: Aaron Holmes
published: 2026-10-21
publisher: The Information
url: "https://www.theinformation.com/articles/bank-hackers-got-claude-dirty-work"
raw: .raw/captured/2026-10-21 The Information - How bank hackers got Claude to do dirty work (notes).md
source_id: src-ccdc3cb261514b36b14e
---

# How Bank Hackers Got Claude to Do Their Dirty Work

Aaron Holmes, The Information, published 2026-10-21.

## Summary

Cybersecurity firm Straiker uncovered how Latin American hacking group CyberCartel automated cyberattacks against financial institutions using commercial AI models including Claude, Grok, and Moonshot's Kimi orchestrated through an external software harness. By using deceptive red-teaming prompts and routing between models, the hackers conducted complex intrusions without needing specialized frontier models like Anthropic's Mythos, mirroring how commercial enterprises use multi-model architectures to optimize costs.

## Key claims

- Cybersecurity firm Straiker found that Latin American hacking group CyberCartel automated financial sector cyberattacks using off-the-shelf commercial AI models instead of restricted frontier systems like Mythos. (§ Harnessing multiple models for cyberattacks: “Straiker revealed that Latin American hacking collective CyberCartel orchestrated automated cyberattacks against financial institutions”) ^clm-b75317f32039e57cbfaf
- CyberCartel developed an orchestration harness combining Anthropic's Claude Opus and Sonnet models with xAI's Grok and Moonshot AI's Kimi. (§ Harnessing multiple models for cyberattacks: “deployed an agent orchestration harness that combined Anthropic's Claude Opus and Sonnet models alongside xAI's Grok and Moonshot's Kimi.”) ^clm-269cafa76209668359e5
- The hacking harness assigned Grok agents to harvest public intelligence and reconnaissance while Claude agents planned and coordinated attack steps. (§ Harnessing multiple models for cyberattacks: “Grok agents were dispatched to scan targets on the web and harvest sensitive intelligence, while Claude agents coordinated”) ^clm-adbeb315ef0b9fb7dbf2
- When Claude refused malicious instructions, CyberCartel tricked the model using simulated internal red-teaming prompts or routed commands to Moonshot's Kimi. (§ Harnessing multiple models for cyberattacks: “harness bypassed safety refusals using deceptive red-teaming prompts or routed tasks to Moonshot's Kimi.”) ^clm-de897a6c8d7fe18e8021
- Security specialist Ken Huang observed that cyberattack potency now resides in orchestration software harnesses rather than single frontier models, enabling attackers to swap models dynamically. (§ Harnessing multiple models for cyberattacks: “Security researcher Ken Huang noted that attack capability now centers on software harnesses rather than individual models”) ^clm-c0490f5e0fcb346f2822
- Multi-model attack harnesses resemble corporate strategies adopted by enterprises like AT&T, which combines open source models with commercial APIs to lower spending on premium frontier models. (§ Corporate defense parallels and pricing implications: “mirrors cost-reduction strategies used by enterprises like AT&T, which blends open-source models with commercial APIs”) ^clm-3b8f3871bbd5658767e4
- Cybersecurity providers including Microsoft and Palo Alto Networks have introduced multi-model defensive systems to match attacker tooling while containing client compute costs. (§ Corporate defense parallels and pricing implications: “Cybersecurity vendors including Microsoft and Palo Alto Networks are offering multi-model defenses”) ^clm-ba45dc81bb1631e203b2

## Entities

[[ATandT|AT&T]], [[Anthropic|Anthropic]], [[CyberCartel|CyberCartel]], [[Microsoft|Microsoft]], [[Moonshot-AI|Moonshot AI]], [[Palo-Alto-Networks|Palo Alto Networks]], [[xAI|xAI]]

## Concepts

[[AI-Agents|AI Agents]]
