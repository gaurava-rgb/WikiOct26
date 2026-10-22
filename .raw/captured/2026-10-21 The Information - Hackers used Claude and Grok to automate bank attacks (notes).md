---
title: "Hackers Used Claude and Grok to Automate Attacks on Banks"
author: Aaron Holmes, Cory Weinberg
publication: The Information
published: 2026-10-21
url: https://www.theinformation.com/articles/hackers-used-claude-grok-fully-automate-attacks-banks
kind: reading-notes
note: "Paraphrased notes with short quotes, taken from Gaurav's subscription. Not the full article text."
---

# Notes: Hackers Used Claude and Grok to Automate Attacks on Banks

The Information, Aaron Holmes and Cory Weinberg, 2026-10-21 (investigative report).

## CyberCartel's automated campaign across Latin America

- Cybercriminal syndicate CyberCartel deployed a network of AI agents to execute automated attacks against more than 400 Latin American financial institutions and payment applications, according to an investigation by cybersecurity firm Straiker.
- The AI agents stole login credentials, harvested customer records, and autonomously accessed bank accounts with minimal human intervention.
- The investigation marks one of the first documented cases of AI models being chained together to execute end-to-end attacks on financial entities.
- Straiker chief executive Ankur Shah warned that offensive AI capabilities currently outpace enterprise defenses, leaving institutions unprepared for automated speed.

## The multi-agent architecture and guardrail evasion

- CyberCartel used Grok agents to scrape targets across the web, four Claude Opus and Sonnet agents to deliberate on attack strategies, and a Claude instance embedded in coding tool Cursor as the lead orchestrator.
- The operation avoided needing Anthropic's top-tier Mythos model, relying instead on API access to commercially available models.
- Attackers bypassed safety filters by framing commands as academic research or benign internal red-team evaluations.
- If Claude models refused an instruction, the harness passed execution to Moonshot's Kimi; if Kimi also refused, the system reverted to deploying conventional malware.
- Following Straiker's notification, Anthropic investigated and terminated the syndicate's API accounts.

## Why it matters for the wiki

- Anthropic entity: documents concrete misuse of Claude Opus and Sonnet alongside prompt injection and jailbreak methods.
- Cursor entity: reveals how developers and bad actors repurpose agentic coding harnesses as autonomous attack controllers.
- AI Agents concept: highlights the shift from human-driven hacking to compute-driven, automated agent swarms.
