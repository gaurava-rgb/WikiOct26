---
title: "How Six AWS Engineers Rebuilt Bedrock to Challenge Microsoft"
author: Catherine Perloff and Kevin McLaughlin
publication: The Information
published: 2026-09-08
url: https://www.theinformation.com/articles/six-aws-engineers-rebuilt-bedrock-challenge-microsoft
kind: reading-notes
note: "Paraphrased notes with short quotes, taken from Gaurav's subscription. Not the full article text."
---

# Notes: How Six AWS Engineers Rebuilt Bedrock to Challenge Microsoft

The Information, Catherine Perloff and Kevin McLaughlin, 2026-09-08 (exclusive).

## The core story

- Bedrock is the AWS service that lets customers run AI models (Claude, and later OpenAI models) inside Amazon's cloud.
- In early 2025 Bedrock was buggy. Customers saw repeated error messages and sometimes waited weeks for computing capacity (per people with knowledge of the issues).
- Senior engineering leader Anthony Liguori and five other senior engineers designed a rebuilt version called **Project Mantle** to fix throttling and errors and let Bedrock scale (per two people). Throttling means the service deliberately slows or limits a customer's requests.
- They built it using Kiro, AWS's in-house AI coding tool.
- Mantle launched in December 2025. A few months later AWS added OpenAI models to Bedrock.

## Results

- Randall Hunt, CTO of AWS consulting firm Caylent, says AWS is now pulling some spending away from Microsoft Azure. Azure used to be the exclusive cloud for OpenAI models.
- Hunt: his financial services clients' AWS spending has grown five times since May.
- Amazon said in July it added more Bedrock customers in the first half of 2026 than in the service's first two years. Q2 Bedrock spending beat all prior quarters combined.
- AWS growth sped up 9 percentage points to 37% in Q2. Azure grew 42%, 2 points faster than the prior quarter.
- AWS spokesperson: Bedrock is "the fastest growing multi-billion-dollar service in AWS history," used by hundreds of thousands of customers.

## How Bedrock got into trouble

- Launched fall 2023, about a year after ChatGPT (late 2022) caught Amazon off guard. Engineers worked 60-hour weeks to build it (per someone who worked on it).
- AWS needed a new service because AI labs guard their model weights (the trained numbers that make up the model) and would not let customers run them directly.
- The rushed build felt "glued together" (per two later staff). It did not fully use its AI chip capacity, causing errors and limits on scale.
- Each customer got a base amount of capacity; going over meant waiting for more. Waits reached up to three weeks (per a former employee).
- Customers complained all through 2025 about throttled access to Anthropic models. AWS leaders worried AI coding startup Lovable might leave.
- An internal sales report in early 2025 said Bedrock's tech problems were hurting deals. Senior leaders called the capacity problems a "disaster" (previously reported).
- Hunt: in 2024 his clients found Anthropic ran up to 63% slower on Bedrock, measured in tokens per second (a speed measure for how fast a model writes text), than going straight to Anthropic's API.
- Dave Treadwell, then an Amazon e-commerce SVP, told AWS leaders in early 2025 that Bedrock's issues made him want to use OpenAI models directly (per two people). A person close to Amazon disputes this. Treadwell is now at AWS.

## What Mantle changed

- Dave Brown, then head of AWS's server business, unveiled Mantle at re:Invent in December. He said the original Bedrock was built like a normal web service, but inference (running a trained model to answer requests) works differently. Brown has since left for Meta.
- Mantle handles "spiky" workloads: tasks that grab lots of compute suddenly, then little.
- Customers can set priority levels for tasks so AWS gives more capacity to what matters most.
- It isolates customers, so one heavy user does not slow others (a spokesperson compared it to many entry gates at a concert venue).
- It works better with an AWS service called Journal, which saves an AI agent's progress so long tasks need not restart after a failure.
- Joe Magerramov, a former AWS VP who helped build it, said inference is closer to a scheduling system than a web service. He followed Brown to Meta last month.
- Mantle is directly compatible with OpenAI and Anthropic APIs, so customers no longer write custom code.
- Wait for extra capacity fell from three weeks to two days by late 2025 (per a former employee). Andy Jassy's 2026 investor letter called Mantle the backbone of Bedrock.
- Later in 2025, Bedrock moved to running mostly on Amazon's own Trainium AI chips, easing reliance on scarce Nvidia chips.

## Caveats

- A manager at one customer using Claude through Mantle reports intermittent outages in recent months, the longest about 11 hours.
- Bojan Jakimovski of consultancy Loka says half a dozen clients moved OpenAI models to Bedrock for faster inference and more throughput at the same cost.

## Why it matters for the wiki

- Model labs vs clouds: once OpenAI models left Azure exclusivity, AWS's rebuilt Bedrock started winning spend from Microsoft.
- Agents beat: long, spiky agent workloads forced a rethink of cloud design, from web service to scheduler.
- Amazon journey beat: a small team plus in-house tools (Kiro, Trainium) fixed a stumble; also a talent leak to Meta (Brown, Magerramov).
