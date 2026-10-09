---
title: "Anthropic's In-House Payments Tech Push Could Chip Away at Stripe"
author: Stephanie Palazzolo
publication: The Information
published: 2026-09-04
url: https://www.theinformation.com/articles/anthropics-house-payments-tech-push-chip-away-stripe
kind: reading-notes
note: "Paraphrased notes with short quotes, taken from Gaurav's subscription. Not the full article text."
---

# Notes: Anthropic's In-House Payments Tech Push Could Chip Away at Stripe

The Information, Stephanie Palazzolo, 2026-09-04 (exclusive). Yueqi Yang contributed.

## The core story

- Recent job postings show Anthropic wants to build more billing, fraud detection and other financial plumbing itself, and is weighing which payment services to build instead of buy.
- Why: soaring usage and complex token-based pricing (charging per unit of text the AI processes) make collecting money hard.
- This could reduce Anthropic's reliance on Stripe. Stripe pitches itself as getting in early with hot startups and growing with them.
- Stripe has promoted that Anthropic uses many of its products beyond core processing: Link checkout, Radar (real-time fraud scoring), invoicing and usage-based billing.
- Anthropic spokesperson: Stripe "has been a strong partner to Anthropic for years," and the work continues. Stripe did not respond.

## What the job posts say

- Anthropic's annualized revenue (current monthly revenue times 12) rose nearly fivefold to almost $45 billion in the five months to May.
- A post for overhauling order management, provisioning, billing and invoicing says the business "is scaling faster than the processes and systems that support it."
- A staff billing engineer would help decide where to keep building on outside platforms and where to build Anthropic's own pieces. Preferred: experience with third-party billing tools and views on where they fall short, plus raising payment approval rates, cutting processing costs and reducing fraud.
- A fraud role covers real-time payment risk checks, tools for disputed charges, and catching people gaming subscriptions and promotions.
- Treasury (managing the company's cash and bank accounts): roles cover centralizing treasury and consolidating banking relationships. One post says the team is building financial apps no vendor has built yet. Buy-versus-build decisions extend to treasury management systems, usually sold by FIS, Kyriba and Trovata.

## Why build in-house

- More control over payment costs and fewer fees to outside firms. Fees are small per transaction but add up, especially with many small developers paying.
- Stripe earns most revenue by taking 2.9% of payment volume plus a fixed per-transaction fee; big customers often pay less. Billing and add-ons are a smaller slice.
- Caveat: fully replacing Stripe would take a long time, especially for processing. The posts do not say Anthropic plans to drop outside processors. Big firms usually keep outsourcing processing but add more providers.

## The wider shift away from Stripe

- Last month OpenAI, a longtime Stripe customer, added Adyen as an extra payment provider (Adyen announced it). Adyen recently bought usage-based billing startup Orb for $335 million.
- Earlier this year OpenAI moved storage of customer card data to an intermediary instead of Stripe's own vault, making it easier to use several processors (The Information reported).
- These moves explain Stripe buying OpenRouter for more than $7 billion. OpenRouter sits between developers and model providers and charges the buyers, giving Stripe another AI revenue stream.
- Stripe's revenue growth sped up to about 33% last year, its fastest since the 2021 pandemic e-commerce boom.
- In January Stripe bought usage-based billing startup Metronome for a reported $1 billion, to meter and charge for AI.
- Shopify added PayPal for some U.S. transactions two years ago and is getting state money transmitter licenses (permits to hold and move customer money), which could cut its need for Stripe.

## Why it matters for the wiki

- AI economics: Anthropic's near-$45B run rate is now big enough that payment fees and billing systems are worth owning.
- Model labs maturing into full companies, building their own back office like big tech did.
- Token-based pricing creates a new billing problem that payment firms (Stripe, Adyen) are racing to solve with acquisitions.
