---
type: concept
title: Shapley Values
status: developing
created: 2026-10-08
updated: 2026-10-16
tags:
  - concept
source_count: 2
---

# Shapley Values

A rule from cooperative game theory for splitting a shared gain among the people who helped make it. Each player gets paid by how much they add on average, across every mix of players with and without them. So a rare, hard-to-replace input earns more than one many others can also supply. Computing it exactly is very costly, so in practice it is estimated.

## Evidence by source

### 2026-05-21 [[2026-05-21-Interview-Parag-Agarwal-Parallel|An Interview with Parallel Founder Parag Agarwal About Valuing Content on the Agentic Web]]

- In the week of May 21, 2026, Parallel launched Index by Parallel, which shows what the content on any given site is worth to agents and pays content creators based on that value. ([[2026-05-21-Interview-Parag-Agarwal-Parallel#^clm-a44560fb776c5d3413a4|cite]])
- Agarwal explains Shapley values with a gloves example: with one seller of a left glove and two sellers of a right glove, the Shapley math pays about 4x more for the scarce left glove. ([[2026-05-21-Interview-Parag-Agarwal-Parallel#^clm-f36d1a0b6c73fdf47279|cite]])
- Agarwal says exact Shapley values cost more to compute than the payment they decide, so Parallel spent a year to a year and a half building a model that estimates them, trained on costly simulations. ([[2026-05-21-Interview-Parag-Agarwal-Parallel#^clm-6f864a396a60e9a69ff2|cite]])
- Index by Parallel gives each site four scores: Impressions, Citations, Value, and Uniqueness; Uniqueness is where the Shapley math rewards content that others do not also supply. ([[2026-05-21-Interview-Parag-Agarwal-Parallel#^clm-9226c02d87ef22445018|cite]])
- Agarwal says Parallel's early data shows unique facts win, with local news and PR Newswire getting outsized value, and plans to publish findings over time. ([[2026-05-21-Interview-Parag-Agarwal-Parallel#^clm-ac2fb07c088e957ec64f|cite]])
- Thompson reports that Stratechery scored highest on Value in the Index but dropped sharply on Uniqueness, while nyc.gov shot up on Uniqueness. ([[2026-05-21-Interview-Parag-Agarwal-Parallel#^clm-9733f7eddc34009b3404|cite]])
- Agarwal says payouts come from a shared pool, like Spotify, that grows with how much agents use the web, and split by Shapley value. ([[2026-05-21-Interview-Parag-Agarwal-Parallel#^clm-e60abd820e9bf9f172d0|cite]])
- Agarwal says Parallel's marketplace covers only data agents use at inference time (when answering), not training data, because no one yet knows how to attribute training data. ([[2026-05-21-Interview-Parag-Agarwal-Parallel#^clm-5618f36d93f27c14caef|cite]])

### 2026-09-29 [[2026-09-29-Google-Is-Paying-About-100-Digital-Publishers-for-AI-Overviews|Google Is Paying About 100 Digital Publishers for AI Overviews]]

- Only a few sources meaningfully improve an answer: if the model checked 100 sites, perhaps only five would count, and topics like anime and gaming seem to earn more. ([[2026-09-29-Google-Is-Paying-About-100-Digital-Publishers-for-AI-Overviews#^clm-0bc143e233f4ca6c2c3b|cite]])
