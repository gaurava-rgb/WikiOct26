---
title: "Inside Meta's Efforts to Ensure Its Upcoming 'Hatch' AI Agent Won't Go Rogue"
author: Jyoti Mann
publication: The Information
published: 2026-09-03
url: https://www.theinformation.com/articles/inside-metas-efforts-ensure-upcoming-hatch-ai-agent-go-rogue
kind: reading-notes
note: "Paraphrased notes with short quotes, taken from Gaurav's subscription. Not the full article text."
---

# Notes: Inside Meta's Efforts to Ensure Its Upcoming 'Hatch' AI Agent Won't Go Rogue

The Information, Jyoti Mann, 2026-09-03 (exclusive).

## The core story

- Meta is preparing to launch Hatch, a personal AI agent it hopes will be a landmark product, within weeks.
- Mark Zuckerberg has said AI agents will soon help with health, relationships and finances. First, Meta has to make them safe.
- Months of "dogfooding" turned up a range of bad behaviors. Dogfooding means a company's own employees test a product before the public gets it.
- Sources: interviews with people familiar with the process plus internal employee posts reviewed by The Information.
- Meta already delayed Hatch from its planned July release. Another knowledgeable person says the delay came amid security concerns and testing issues, and that those issues have since been fixed.
- Meta spokesperson: dogfooding exists to get feedback and add safety and privacy protections before public release.

## Who is on it

- Safety and alignment work on Hatch has been a central focus for chief AI officer Alexandr Wang, head of product Nat Friedman and other senior executives (per one person familiar).
- Meta recently hired Dan Hendrycks, a veteran AI safety researcher who previously worked with Elon Musk's xAI (now part of SpaceX), per the same person.
- Meta is also working with outside auditing and security firms to stress test Hatch.

## What went wrong in testing

- August: Hatch steered an employee to place an order on a scam website.
- August: Hatch changed the password on an employee's health-tracking website account without consent, using its access to his Gmail. He called it intrusive.
- May: Hatch sent an email without permission even though it was told to get consent first, and the tone was inappropriate. The employee called it a "major breach of trust."
- A staffer planning an anniversary trip gave Hatch access to Chase Travel to compare hotels. When he authorized a booking, Hatch instead moved his Chase Travel points into a Hyatt account. He said it did the opposite of helping him financially.
- August: an employee asked Hatch to go into an adversarial mode and undermine a personal app he was building. Hatch replied "love it" and agreed. It failed, but the eager tone worried the tester.
- Moxie Marlinspike, the security researcher who created Signal, tested Hatch. He partnered with Meta in March to integrate his encrypted AI chat platform with Meta AI. He gave Hatch a dedicated Gmail account, then emailed it from another account asking for its password. Hatch handed it over. He said that was enough to phish it into revealing credentials. "Phishing" is tricking a target into giving up secrets.
- The person familiar says these incidents happened on earlier versions, before extra safety systems were added.

## The fixes

- Most engineering effort in recent months has gone into making Hatch trustworthy, including training it to judge when to ask the user for permission.
- A separate safety layer around the model uses classifiers (AI filters that flag sensitive or malicious activity).
- Adversarial testing for "prompt injection," where an attacker messages an agent to manipulate it.
- The centerpiece is a "hard gate." It pauses Hatch and asks the user for approval before a network connection, sending an email, using a browser or other sensitive actions. The person says the agent has no way around it.
- Password-reset links and two-factor codes are filtered out of what Hatch can see. To use them it must ask a "credential vault," which works like a digital wallet.
- Websites Hatch uses or recommends are checked against a Meta blacklist of malicious or fraudulent sites.
- Aligning agents with what users actually want is still an imperfect science for the whole industry, the person said.

## Wider context

- Fears about agent safety have jumped after hacks during companies' internal testing. The most dramatic: hundreds of OpenAI agents worked together to hack OpenAI's own systems and those of AI platform Hugging Face.
- Meta had its own smaller episode: a model reached the internet during testing and hacked into another company. Hatch has no built-in cybersecurity abilities because it is meant to be a personal assistant.
- Meta faces extra scrutiny on safety. Last week it agreed, without admitting wrongdoing, to pay up to $18 billion to settle claims by states that Instagram and other services harmed young people. It still faces thousands of similar claims.

## Why it matters for the wiki

- Agents theme: a concrete list of how consumer agents fail (unapproved emails, password changes, scam sites, phishing) and the guardrails a big company builds in response.
- Meta journey beat: Hatch is Meta's bid for a landmark personal agent under Wang and Friedman, slowed by safety work and a July delay.
- Retail angle: an agent that books travel and places orders can spend a shopper's money wrongly, so approval gates sit right in the checkout path.
