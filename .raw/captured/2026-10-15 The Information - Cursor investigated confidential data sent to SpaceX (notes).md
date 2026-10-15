---
title: "Cursor Staff Investigated Whether Confidential Data Reached SpaceX for AI Training"
author: Grace Kay
publication: The Information
published: 2026-10-15
url: https://www.theinformation.com/articles/cursor-staff-investigated-whether-confidential-data-reached-spacex-ai-training
kind: reading-notes
note: "Paraphrased notes with short quotes, taken from Gaurav's subscription. Not the full article text."
---

# Notes: Cursor Staff Investigated Whether Confidential Data Reached SpaceX for AI Training

The Information, Grace Kay, 2026-10-15.

## The core story

- Cursor engineers investigated whether internal testing data containing confidential customer, supplier, and partner information had been sent to SpaceX's AI unit for model training.
- The investigation occurred in late July 2026, weeks before SpaceX's AI unit (SpaceXSI) launched its Grok Bot autonomous personal agent.
- A Cursor attorney warned employees in internal messages that using this testing data for training could trigger a major customer trust crisis.
- The lawyer noted that broad usage of the tool meant datasets included third-party confidential details that Cursor arguably had no legal right to use for model training.
- While Cursor did not share the formal conclusion of the inquiry, the company changed policies to exclude employee usage data from future training datasets.

## Grok Bot development and internal testing

- Cursor led the development of Grok Bot, an always-on AI workplace assistant intended to expand the startup's footprint into general enterprise workflows beyond software coding.
- The product was code-named Sand inside Cursor and distributed to staff for internal testing around June 2026.
- Staff members used the agent across departments including sales, technical recruiting, and market research, granting the tool autonomous access to corporate databases and communications.
- Testing exposed Sand to sensitive negotiations with prospective hires and enterprise customer records.
- Several employees accessed Sand using personal email accounts, which made it harder to trace and remove their data from training pools.
- Cursor responded by mandating corporate email addresses for tool access and barring employee activity from model training.

## Previous customer data leaks on marketing sites

- Earlier in 2026, Cursor sales and marketing staff inadvertently leaked sensitive enterprise customer data through public websites deployed on Vercel.
- The internal web pages were designed to manage client relationships with major companies including Verizon, Bosch, and Coupa.
- The Verizon portal contained organizational charts of technical managers, lists of top Cursor users, user email addresses, and specific software spending figures.
- Although protected by passwords, the passwords and confidential customer records were hardcoded in publicly readable front-end source code.
- Cursor engineers created an internal incident response channel titled "A ton of gtm sites that leak customer/internal data" to remove the exposed websites.

## Security track record across SpaceX and xAI

- SpaceX and xAI have experienced repeated data security and credential exposure issues.
- In March 2025, a SpaceXSI employee exposed an internal Grok application programming interface key after accidentally uploading a test script to a public GitHub repository.
- In summer 2026, an external researcher found that developer tool Grok Build uploaded entire Git code repositories to company Google Cloud storage buckets.
- In response to that leak, xAI disabled repository uploads, open-sourced the software, and Elon Musk stated all user uploads would be completely erased.
- SpaceX completed its $60 billion acquisition of Cursor in mid-August 2026 to push into lucrative enterprise AI markets.

## Why it matters for the wiki

- Connects to [[journeys/openai-journey-2026|OpenAI, 2026]] and [[stories/ai-shift-2024-2026|The AI shift, 2024 to 2026]]: shows how autonomous enterprise agents with file access create data leakage hazards that threaten enterprise adoption.
- Informs [[concepts/Zero-Data-Retention|Zero Data Retention]]: demonstrates why enterprise customers insist on strict data boundaries, as internal agent testing and loose marketing portals expose customer spend and employee records.
- Informs [[concepts/AI-Agents|AI Agents]]: illustrates the trade-off between giving autonomous agents wide system access and protecting confidential enterprise information.
