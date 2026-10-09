---
type: source
title: "Fable 5.1, Enterprise Frontier Safeguards"
status: evergreen
created: 2026-09-29
updated: 2026-09-29
tags:
  - source
  - source/update
author: Ben Thompson
published: 2026-09-02
publisher: Stratechery
url: "https://stratechery.com/2026/fable-5-1-enterprise-frontier-safeguards/"
raw: ".raw/captured/Fable 5.1, Enterprise Frontier Safeguards.md"
source_id: src-40778f5663ced98b8e45
---

# Fable 5.1, Enterprise Frontier Safeguards

Ben Thompson, Stratechery, published 2026-09-02.

## Summary

Anthropic released Fable 5.1, the same model as Mythos 5.1 but with lighter safeguards, and cut the price of cache reads by 75%. Thompson argues cheaper cache is a win both for enterprise buyers who pay per token and for Anthropic's margins on subscriptions. Anthropic also dropped its hated 30-day data retention rule for Fable and will offer Enterprise Frontier Safeguards, which keep data in the customer's own cloud, with zero retention in the meantime. Thompson reads this as proof that high prices and the retention rule held back business use of Fable 5, and that customer pushback and the need to make money keep Anthropic in check.

## Key claims

- Anthropic says Claude Fable 5.1 and Claude Mythos 5.1 are the same model with different levels of safeguards; Fable 5.1 is generally available, while Mythos 5.1 is only offered through trusted access programs for cybersecurity and life sciences work. (§ Fable 5.1: “Claude Fable 5.1 and Claude Mythos 5.1 are the same model, but with different levels of safeguards”) ^clm-147520481e0508800242
- Anthropic says Fable 5.1 is better than Fable 5 at long, complex coding tasks and at scientific work such as experiment design and reading dense diagrams and tables. (§ Fable 5.1: “is more skilled at carrying out lengthy, complicated computer programming tasks”) ^clm-557f8083761a6dce87de
- Bloomberg reports that cheaper, improving open-weight models from China are pushing US model makers like Anthropic on price as companies try to rein in AI costs. (§ Fable 5.1: “open-weight, lower cost models from China are rapidly improving”) ^clm-5d1bdf9534fc172f13d5
- Anthropic keeps the same per-token price for Fable 5.1 as Fable 5 but cuts the price of cache reads (tokens the model re-reads after already processing them) by 75%. (§ Fable 5.1: “the 75% price reduction it’s offering on this part of the process”) ^clm-bfab7a40ad3d0cd2716c
- Dianne Penn of Anthropic says cache reads can be half or more of the tokens used in some long, complex tasks. (§ Fable 5.1: “The process can account for half or more of the tokens used”) ^clm-3523dee2eaf5f0d9beeb
- Anthropic estimates Fable 5.1 will cost about 25% less than Fable 5 for typical token-billed workloads, and up to about 45% less for highly agentic work. (§ Fable 5.1: “Fable 5.1 will cost an estimated 25% less than Fable 5 for typical workloads”) ^clm-9e376769b4b17d3c5efe
- Thompson argues cache matters most for agentic workflows, because tool definitions and schemas are loaded into the context window and are the same across all users. (§ Fable 5.1: “Cache is particularly important for agentic workflows, which involve a lot of tool use”) ^clm-d5a543435c315f024803
- Thompson argues cache is close to free compared with generation, so a better cache layer lets Anthropic credibly lower the price per task even while the price per generated token stays the same. (§ Fable 5.1: “the price-per-task is lower even if the price-per-generated-token is the same”) ^clm-1b092c160be42fe95f10
- Thompson argues the price cut applies only where usage is billed by token, not to subscriptions, so lower serving costs raise Anthropic's margins on subscriptions and make better caching a win on both sides of the business. (§ Fable 5.1: “any savings they can achieve increase their margins on subscriptions”) ^clm-74e0bf8a2b3cad897037
- Anthropic introduced a rule in June 2026, with Fable 5 and Mythos 5, requiring 30-day retention of all traffic on those models to defend against misuse and cyberattacks, while pledging not to use the data for training. (§ Enterprise Frontier Safeguards: “it would require 30-day retention for all traffic on those models”) ^clm-06734bbff379e00ef7d7
- Anthropic announced it will replace the retention policy with Enterprise Frontier Safeguards after customer feedback; Kate Jensen said the company spent hundreds of hours with customers on the new approach. (§ Enterprise Frontier Safeguards: “the company spent hundreds of hours working with customers to develop another solution”) ^clm-b383ac45a4a58c129c55
- Enterprise Frontier Safeguards will be free, will let businesses control how their data is reviewed and stored with automated safety monitoring and no Anthropic human review, and will work whether customers use Anthropic directly or through a cloud provider. (§ Enterprise Frontier Safeguards: “The company said it will not charge for Enterprise Frontier Safeguards”) ^clm-9648ec5a6e48116f3e2b
- Enterprise Frontier Safeguards store data in cloud infrastructure controlled entirely by the customer; it rolls out in phases starting later in fall 2026, and until then eligible customers can use Fable 5.1 with zero data retention. (§ Enterprise Frontier Safeguards: “Until EFS is available, eligible customers will be able to use Fable 5.1 with zero data retention”) ^clm-43f9280cddc130b24445
- Ramp data showed that one month after launch, Fable 5 made up only 6% of tokens businesses bought from Anthropic and 11.4% of dollars spent on Anthropic models. (§ Enterprise Frontier Safeguards: “Fable 5 has made up only 6% of tokens businesses purchased from Anthropic”) ^clm-ecfa3c4cb141a7e291bb
- Per Ramp, OpenAI's flagship GPT-5.6 Sol made up 25% of OpenAI tokens and 23% of OpenAI spend, and in July Fable 5 generated about 75% as much model-attributed spend as GPT-5.6 Sol. (§ Enterprise Frontier Safeguards: “Fable 5 generated approximately 75% as much model-attributed spend as GPT-5.6 Sol”) ^clm-428370793e928b3a6013
- Ramp put Fable 5's price at roughly $10 per million tokens, twice the price of GPT-5.6 Sol, and argued this marks an upper bound on what businesses will pay for AI performance. (§ Enterprise Frontier Safeguards: “we’ve found a new upper bound for how much businesses are willing to spend on AI”) ^clm-1fb817e7e354d9326d7c
- Prediction: Ramp argued labs must beat even Fable 5 on performance while keeping rivals from getting close, which looks harder as open source models close to only a few months behind. (§ Enterprise Frontier Safeguards: “open source models catch up to being only a few months behind”) ^clm-797b8db92c0d9aebaa47
- Thompson argues price was probably the biggest reason for Fable 5's low business uptake, citing his own shock at the cost of finishing a project on credits after hitting subscription limits. (§ Enterprise Frontier Safeguards: “price was probably the biggest reason for Fable’s relatively low penetration”) ^clm-f349f511bd5c2f1441b9
- Thompson argues anything but zero data retention is a no-go for most large enterprises, so the retention rule also hurt Fable adoption. (§ Enterprise Frontier Safeguards: “Anything but a zero data retention policy is, for most large enterprises, simply a no-go”) ^clm-bcca8278e8628748800f
- Thompson argues the retention rule's biggest effect was to help rivals like Microsoft, with Satya Nadella publicly pressing on sharing data with frontier labs and Alex Karp giving a wild interview on the issue. (§ Enterprise Frontier Safeguards: “putting wind in the sails of companies like Microsoft”) ^clm-ef7ac383273583fa046c
- Prediction: Thompson earlier predicted that if the retention rule did not cost Anthropic many customers, Anthropic would eventually start using the retained data, since it is too valuable to its goals. (§ Enterprise Frontier Safeguards: “I suspect it’s only a matter of time until they start using the data”) ^clm-0bca1a37754d97164833
- Thompson says Anthropic may not have lost customers under the retention rule, but growth slowed and Fable usage was stagnant, which led to Enterprise Frontier Safeguards. (§ Enterprise Frontier Safeguards: “Anthropic might not have lost customers, but”) ^clm-94b654b5b22727de0b18
- Thompson argues that reverting to true zero retention until EFS ships shows the safety concerns were not so great, supporting his suspicion about where the retention policy was heading. (§ Enterprise Frontier Safeguards: “Apparently the safety concerns aren’t so great that Anthropic can’t revert”) ^clm-6ec25e65bf9cfe5a8580
- Thompson argues the episode shows competition works and customers can push back, and that the need to make money curbs Anthropic's worst impulses; for-profit enterprise is the best alignment organizing principle. (§ Enterprise Frontier Safeguards: “For-profit enterprise is the best alignment organizing principle there is”) ^clm-76e3d8d465feabd41fa7
- Thompson notes the Fable 5.1 release topped Techmeme with many X posts, while the Enterprise Frontier Safeguards news sat halfway down the page with mostly LinkedIn posts. (§ Enterprise Frontier Safeguards: “this item was buried halfway down the page”) ^clm-a7a771d92725edd13098

## Entities

Alex Karp, [[Anthropic|Anthropic]], [[Ben-Thompson|Ben Thompson]], Dianne Penn, Kate Jensen, [[Microsoft|Microsoft]], [[OpenAI|OpenAI]], [[Ramp|Ramp]], [[Satya-Nadella|Satya Nadella]]

## Concepts

[[AI-Agents|AI Agents]], [[Commodity-Cost-Advantage|Winning a Commodity Market on Cost]], Zero Data Retention
