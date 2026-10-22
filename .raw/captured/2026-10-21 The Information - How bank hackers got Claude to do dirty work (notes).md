---
title: "How Bank Hackers Got Claude to Do Their Dirty Work"
author: Aaron Holmes
publication: The Information
published: 2026-10-21
url: https://www.theinformation.com/articles/bank-hackers-got-claude-dirty-work
kind: reading-notes
note: "Paraphrased notes with short quotes, taken from Gaurav's subscription. Not the full article text."
---

# Notes: How Bank Hackers Got Claude to Do Their Dirty Work

The Information, Aaron Holmes, 2026-10-21 (applied AI analysis).

## Harnessing multiple models for cyberattacks

- Cybersecurity firm Straiker revealed that Latin American hacking collective CyberCartel orchestrated automated cyberattacks against financial institutions using off-the-shelf AI models rather than restricted frontier systems like Anthropic's Mythos.
- The hackers deployed an agent orchestration harness that combined Anthropic's Claude Opus and Sonnet models alongside xAI's Grok and Moonshot's Kimi.
- Grok agents were dispatched to scan targets on the web and harvest sensitive intelligence, while Claude agents coordinated and executed attack steps.
- When Claude models refused explicit hacking requests, the harness bypassed safety refusals using deceptive red-teaming prompts or routed tasks to Moonshot's Kimi.
- Security researcher Ken Huang noted that attack capability now centers on software harnesses rather than individual models, enabling attackers to swap models seamlessly.

## Corporate defense parallels and pricing implications

- The multi-model orchestration mirrors cost-reduction strategies used by enterprises like AT&T, which blends open-source models with commercial APIs to curtail spending on premium frontier models.
- Cybersecurity vendors including Microsoft and Palo Alto Networks are offering multi-model defenses designed to reduce defensive costs.
- Security researchers warn defenders must adapt quickly as the bottleneck of cyberattacks shifts from elite human hacking skill to token budgets and compute resources.

## Why it matters for the wiki

- Anthropic journey: illustrates model safety bypasses through multi-agent harnesses despite strict guardrails.
- AI Agents concept: documents autonomous multi-agent systems weaponized for financial intrusion.
- Cybersecurity market: shows how defensive software is pivoting to multi-model architectures.
