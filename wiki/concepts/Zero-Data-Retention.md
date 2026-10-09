---
type: concept
title: Zero Data Retention
status: developing
created: 2026-09-29
updated: 2026-10-09
tags:
  - concept
source_count: 4
---

# Zero Data Retention

A promise from an AI provider that it will not keep a customer's prompts and outputs after a request is done. For most large companies this is a must before they send sensitive work to a model. Fights over retention are fights over trust and over who gets to see and later use the data.

## Evidence by source

### 2026-07-09 [[2026-07-09-Muse-Image-Grok-4-5-Alex-Karp-on-CNBC|Muse Image, Grok 4.5, Alex Karp on CNBC]]

- Karp said closed frontier models could also work if clients can ask basic questions such as whether the lab keeps their data or will enter their business. ([[2026-07-09-Muse-Image-Grok-4-5-Alex-Karp-on-CNBC#^clm-229825687d8e1240cd67|cite]])
- Thompson calls Anthropic's Fable-era change to retain data from all customers, including enterprise, the most underrated part of the Fable release. ([[2026-07-09-Muse-Image-Grok-4-5-Alex-Karp-on-CNBC#^clm-82cd67bed7b32d756caf|cite]])
- Prediction: Thompson predicts that if the retention policy does not cost Anthropic many customers, it is only a matter of time until Anthropic trains on that data, despite its pledge not to. ([[2026-07-09-Muse-Image-Grok-4-5-Alex-Karp-on-CNBC#^clm-8215bb9edb0b08cd828a|cite]])

### 2026-09-02 [[2026-09-02-Fable-5-1-Enterprise-Frontier-Safeguards|Fable 5.1, Enterprise Frontier Safeguards]]

- Anthropic introduced a rule in June 2026, with Fable 5 and Mythos 5, requiring 30-day retention of all traffic on those models to defend against misuse and cyberattacks, while pledging not to use the data for training. ([[2026-09-02-Fable-5-1-Enterprise-Frontier-Safeguards#^clm-06734bbff379e00ef7d7|cite]])
- Anthropic announced it will replace the retention policy with Enterprise Frontier Safeguards after customer feedback; Kate Jensen said the company spent hundreds of hours with customers on the new approach. ([[2026-09-02-Fable-5-1-Enterprise-Frontier-Safeguards#^clm-b383ac45a4a58c129c55|cite]])
- Enterprise Frontier Safeguards will be free, will let businesses control how their data is reviewed and stored with automated safety monitoring and no Anthropic human review, and will work whether customers use Anthropic directly or through a cloud provider. ([[2026-09-02-Fable-5-1-Enterprise-Frontier-Safeguards#^clm-9648ec5a6e48116f3e2b|cite]])
- Enterprise Frontier Safeguards store data in cloud infrastructure controlled entirely by the customer; it rolls out in phases starting later in fall 2026, and until then eligible customers can use Fable 5.1 with zero data retention. ([[2026-09-02-Fable-5-1-Enterprise-Frontier-Safeguards#^clm-43f9280cddc130b24445|cite]])
- Thompson argues anything but zero data retention is a no-go for most large enterprises, so the retention rule also hurt Fable adoption. ([[2026-09-02-Fable-5-1-Enterprise-Frontier-Safeguards#^clm-bcca8278e8628748800f|cite]])
- Thompson argues the retention rule's biggest effect was to help rivals like Microsoft, with Satya Nadella publicly pressing on sharing data with frontier labs and Alex Karp giving a wild interview on the issue. ([[2026-09-02-Fable-5-1-Enterprise-Frontier-Safeguards#^clm-ef7ac383273583fa046c|cite]])
- Prediction: Thompson earlier predicted that if the retention rule did not cost Anthropic many customers, Anthropic would eventually start using the retained data, since it is too valuable to its goals. ([[2026-09-02-Fable-5-1-Enterprise-Frontier-Safeguards#^clm-0bca1a37754d97164833|cite]])
- Thompson says Anthropic may not have lost customers under the retention rule, but growth slowed and Fable usage was stagnant, which led to Enterprise Frontier Safeguards. ([[2026-09-02-Fable-5-1-Enterprise-Frontier-Safeguards#^clm-94b654b5b22727de0b18|cite]])
- Thompson argues that reverting to true zero retention until EFS ships shows the safety concerns were not so great, supporting his suspicion about where the retention policy was heading. ([[2026-09-02-Fable-5-1-Enterprise-Frontier-Safeguards#^clm-6ec25e65bf9cfe5a8580|cite]])
- Thompson argues the episode shows competition works and customers can push back, and that the need to make money curbs Anthropic's worst impulses; for-profit enterprise is the best alignment organizing principle. ([[2026-09-02-Fable-5-1-Enterprise-Frontier-Safeguards#^clm-76e3d8d465feabd41fa7|cite]])

### 2026-09-14 [[2026-09-14-Anthropic-Data-Fears-Prompt-Nvidia-Palantir-and-Booz-Allen-to-Restrict-Model-Use|Anthropic Data Fears Prompt Nvidia, Palantir and Booz Allen to Restrict Model Use]]

- In June 2026 Anthropic changed its policy for its flagship Fable model to give itself the right to keep logs of customer use on a rolling 30-day basis, saying this helps defend against complex, novel attacks. ([[2026-09-14-Anthropic-Data-Fears-Prompt-Nvidia-Palantir-and-Booz-Allen-to-Restrict-Model-Use#^clm-9119ddf4f1357b57d17c|cite]])
- Before the June change, Anthropic had given some business customers zero data retention, meaning it did not store their data at all. ([[2026-09-14-Anthropic-Data-Fears-Prompt-Nvidia-Palantir-and-Booz-Allen-to-Restrict-Model-Use#^clm-35cb31591bc49d60b61f|cite]])
- OpenAI let customers store safety logs from GPT-5.6-Cyber users on their own servers in August 2026, and after customer blowback Anthropic launched a similar self-storage option in September, built with more than 100 customers. ([[2026-09-14-Anthropic-Data-Fears-Prompt-Nvidia-Palantir-and-Booz-Allen-to-Restrict-Model-Use#^clm-218eb3774e5c59ef832e|cite]])
- Palantir, which resells Anthropic models, will not offer Fable to its clients until Anthropic gives zero data retention it cannot later revoke. ([[2026-09-14-Anthropic-Data-Fears-Prompt-Nvidia-Palantir-and-Booz-Allen-to-Restrict-Model-Use#^clm-1fefa158949545de3016|cite]])
- Palantir and some others say they have zero data retention access to OpenAI's GPT-6 Astra, which Palantir now offers. ([[2026-09-14-Anthropic-Data-Fears-Prompt-Nvidia-Palantir-and-Booz-Allen-to-Restrict-Model-Use#^clm-d258b7d99aabeeb8d652|cite]])
- A large US utility dropped plans to test Fable for running core power infrastructure after Anthropic refused nonrevocable zero data retention. ([[2026-09-14-Anthropic-Data-Fears-Prompt-Nvidia-Palantir-and-Booz-Allen-to-Restrict-Model-Use#^clm-410fcedc16acddf244f5|cite]])

### 2026-09-28 [[2026-09-28-Anthropic-Moves-to-Cut-Off-Discounts-When-Customers-Hit-Their-Cap|Anthropic Moves to Cut Off Discounts When Customers Hit Their Cap]]

- Worries that the labs could learn from customers' intellectual property have led Palantir, Nvidia and Booz Allen Hamilton to demand guarantees or cut use of the most advanced models. ([[2026-09-28-Anthropic-Moves-to-Cut-Off-Discounts-When-Customers-Hit-Their-Cap#^clm-5172f1f9fb58f6ade051|cite]])
