---
title: "Anthropic Data Fears Prompt Nvidia, Palantir and Booz Allen to Restrict Model Use"
author: Laura Bratton and Aaron Holmes
publication: The Information
published: 2026-09-14
url: https://www.theinformation.com/articles/anthropic-data-fears-prompt-nvidia-palantir-booz-allen-restrict-model-use
kind: reading-notes
note: "Paraphrased notes with short quotes, taken from Gaurav's subscription. Not the full article text."
---

# Notes: Anthropic Data Fears Prompt Nvidia, Palantir and Booz Allen to Restrict Model Use

The Information, Laura Bratton and Aaron Holmes (Stephanie Palazzolo contributed), 2026-09-14 (exclusive). Updated with more OpenAI comment.

## The core story

- Fear is rising that Anthropic or OpenAI could learn from customers' intellectual property. Firms doing sensitive work (Palantir, Nvidia, Booz Allen Hamilton) are demanding new guarantees, or cutting or ending use of the labs' top models.
- Trigger at Anthropic: a June policy change for its flagship Fable model. Anthropic gave itself the right to keep logs of customer use on a rolling 30-day basis, saying this helps it defend against complex, novel attacks.
- Before that, Anthropic had given some business customers zero data retention (ZDR), meaning it did not store their data at all.
- OpenAI, meanwhile, is defending against claims it may have used a user's data to help reach a major math breakthrough.

## What the labs say they collect

- Both say that by default they do not train on enterprise customers' inputs or outputs unless customers opt in. Individual users must opt out manually.
- Both collect some metadata (data about usage, not the content itself) from corporate customers. What exactly is unclear.
- OpenAI says its metadata is de-identified (stripped of anything naming the customer) and not used to improve models.
- OpenAI Chief Research Officer Mark Chen posted on X Tuesday that such data helps improve models, including the AI that solved the Navier-Stokes math problem. A spokesperson later said Chen meant data customers chose to share, and that an internal check found no data from Navier-Stokes researchers in the past two years was used.
- Anthropic uses aggregated, anonymized usage data (which features work better or worse) to improve products, but says it does not train models on it.
- C Spire, a telecom, bars both labs from training on its data but lets them collect technical usage data. Chief AI Officer Fernando Higuera called it "a blank spot in our radar," not a red flag. An OpenAI official said it does not train on models' "chains of thought" (the step-by-step reasoning a model writes while working).

## Retention policy back and forth

- OpenAI said it would keep some logs from GPT-5.6-Cyber users for safety, then in August let customers store those logs on their own servers.
- After customer blowback, Anthropic this month launched a similar self-storage option, rolling out in phases this fall. It says it built it with more than 100 customers, but others must request access, and Anthropic kept the right to end the option at any time.

## Customer by customer

- **Palantir**: resells Anthropic models in its software. It had earlier won irrevocable ZDR guarantees across all models (per a person familiar). The June change reopened talks. Palantir will not offer Fable to clients until Anthropic gives ZDR it cannot later revoke. Clients can still buy Fable directly.
- CEO Alex Karp said last week enterprises are tired of AI labs abusing them. Palantir handed out a booklet titled "How to Avoid Transferring Your Alpha to a Hosted Model Provider" on negotiating ZDR. Palantir and some others say they have ZDR access to OpenAI's GPT-6 Astra, which Palantir now offers.
- The article notes Palantir's warnings are self-serving: it wants to be the buffer between businesses and the labs. Microsoft, Salesforce and others make similar pitches.
- **Nvidia**: uses Fable only for less sensitive work such as open-source projects. Justin Boitano, VP of enterprise AI, said ZDR should be on by default. Sensitive work, like AI supply chain monitoring, runs on Nvidia's own Nemotron models. Nvidia has invested in Anthropic, which is also a big Nvidia hardware buyer.
- **Booz Allen Hamilton**: an early user of Anthropic's Mythos for finding cyber holes, but bars staff from using Fable on its proprietary cybersecurity software. CTO Bill Vass worries Fable "might be learning from some of our code," though he says most cases are not a concern.
- **A large U.S. utility**: dropped plans to test Fable for running core power infrastructure serving millions of homes after Anthropic refused nonrevocable ZDR. Still uses Anthropic for finance and HR tasks like onboarding.
- **Novo Nordisk**: uses Claude for public documents and generic drafts but bans feeding it proprietary data.
- **Northrop Grumman**: runs open-source models on air-gapped servers (machines cut off from the internet) for coding and research, using models from Poolside, Luminary and Nvidia. It hired ex-Microsoft AI researchers Fahad Khan and Praveen Palanisamy to help lead the effort.

## Microsoft pounces

- Microsoft is using the fears to lure OpenAI and Anthropic clients (per people involved).
- It recently offered one large client privately managed servers that send no data to outside AI providers, costing millions over several years. The client is still deciding.

## Why it matters for the wiki

- Model labs vs clouds: data trust becomes a wedge for Microsoft and Palantir to sit between enterprises and the labs.
- AI economics: as labs sell their own apps, big customers see them as possible competitors, which caps how much sensitive work they hand over.
- Compute and deployment: air-gapped, self-hosted open models (Northrop, Nvidia Nemotron) are a real alternative for sensitive work.
