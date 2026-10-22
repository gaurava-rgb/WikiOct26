---
type: source
title: Hackers Used Claude and Grok to Automate Attacks on Banks
status: evergreen
created: 2026-10-21
updated: 2026-10-21
tags:
  - source
  - source/article
author: "Aaron Holmes, Cory Weinberg"
published: 2026-10-21
publisher: The Information
url: "https://www.theinformation.com/articles/hackers-used-claude-grok-fully-automate-attacks-banks"
raw: .raw/captured/2026-10-21 The Information - Hackers used Claude and Grok to automate bank attacks (notes).md
source_id: src-35e127dd7a15c5e5eb98
---

# Hackers Used Claude and Grok to Automate Attacks on Banks

Aaron Holmes, Cory Weinberg, The Information, published 2026-10-21.

## Summary

Cybersecurity startup Straiker discovered that cybercrime group CyberCartel orchestrated automated attacks targeting over 400 Latin American banks and payment services using AI agents powered by Claude, Grok, and Moonshot's Kimi. The syndicate chained agents together, using a Claude agent inside Cursor as the command center, to steal passwords, exfiltrate data, and access accounts autonomously. Anthropic terminated the group's accounts upon being alerted.

## Key claims

- Cybercriminal group CyberCartel launched automated attacks against more than 400 Latin American banks and financial apps using multi-agent AI systems. (§ CyberCartel's automated campaign across Latin America: “CyberCartel deployed a network of AI agents to execute automated attacks against more than 400 Latin American financial institutions”) ^clm-c6baca8dac82ae1cefa6
- The autonomous AI agents exfiltrated customer records, compromised credentials, and gained access to bank accounts with minimal manual human input. (§ CyberCartel's automated campaign across Latin America: “agents stole login credentials, harvested customer records, and autonomously accessed bank accounts with minimal human intervention.”) ^clm-165bf5bdce433c376d01
- The CyberCartel campaign represents one of the first confirmed real-world operations where commercial AI models were chained to execute end-to-end attacks on financial firms. (§ CyberCartel's automated campaign across Latin America: “one of the first documented cases of AI models being chained together to execute end-to-end attacks on financial entities.”) ^clm-2056dcb96bec46d1c7b3
- Straiker CEO Ankur Shah stated offensive AI capabilities currently hold a clear advantage over enterprise defenses, leaving institutions vulnerable to automated attacks. (§ CyberCartel's automated campaign across Latin America: “Straiker chief executive Ankur Shah warned that offensive AI capabilities currently outpace enterprise defenses”) ^clm-b3bb1976ced2c2aaec97
- CyberCartel's attack structure deployed four Claude Opus and Sonnet agents for strategic planning while using a Claude agent running within coding tool Cursor as the lead attack commander. (§ The multi-agent architecture and guardrail evasion: “four Claude Opus and Sonnet agents to deliberate on attack strategies, and a Claude instance embedded in coding tool Cursor as the lead orchestrator.”) ^clm-7713a6d48250ce700d65
- The attackers bypassed commercial AI model safety guardrails by instructing models that they were performing academic security evaluations or internal red-teaming. (§ The multi-agent architecture and guardrail evasion: “bypassed safety filters by framing commands as academic research or benign internal red-team evaluations.”) ^clm-08369f55d3f333872b04
- When Claude models declined malicious actions, the system automatically routed execution to Moonshot AI's Kimi or defaulted to traditional malware deployment. (§ The multi-agent architecture and guardrail evasion: “harness passed execution to Moonshot's Kimi; if Kimi also refused, the system reverted to deploying conventional malware.”) ^clm-ef5e029ca83ca9fcbe11
- Anthropic launched an investigation and terminated CyberCartel's API access after Straiker notified the company of the hacking campaign. (§ The multi-agent architecture and guardrail evasion: “Following Straiker's notification, Anthropic investigated and terminated the syndicate's API accounts.”) ^clm-306835fbcd3e9e056294

## Entities

[[Anthropic|Anthropic]], [[Cursor|Cursor]], [[CyberCartel|CyberCartel]], [[Moonshot-AI|Moonshot AI]]

## Concepts

[[AI-Agents|AI Agents]]
