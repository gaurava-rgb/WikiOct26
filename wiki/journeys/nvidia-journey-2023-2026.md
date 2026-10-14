---
type: journey
title: "Nvidia, 2023 to 2026: selling every chip it can make"
status: developing
created: 2026-10-13
updated: 2026-10-13
tags:
  - journey
  - nvidia
---

# Nvidia, 2023 to 2026: selling every chip it can make

**Thesis:** Nvidia sells far more than chips. It sells whole systems, and in 2026 it began lending money and buying companies so that many buyers, not a few giants, keep needing it. This era is the selling: demand outran supply, and the biggest buyers began building their own chips. Part of the [[journeys/nvidia-journey|Nvidia journey]]; next era: [[journeys/nvidia-journey-late-2026|Nvidia, late 2026]].

## The story so far

Demand for scarce, costly AI chips helped make Nvidia a company worth over a trillion dollars ([[2025-Gallaugher-Ch08-Amazon|Gallaugher ch.8]], p.298). Since then its sales are capped by how many chips its suppliers can make, not by how many buyers want them ([[2026-09-01-Nvidia-Earnings-Dollars-Per-Gigawatt-Open-and-Hugging-Face|Nvidia Earnings, Aug]]). Its biggest buyers, the cloud giants, also build their own chips to need it less ([[2026-09-13-Nvidias-Growing-Dependence-On-a-Few-Big-Customers|Nvidia's Few Big Customers]]).

## Hook: the lab that got away

For years Nvidia sold almost nothing to Anthropic, because Anthropic ran on Google's TPU chips and Amazon's Trainium chips after taking their money ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia Earnings, May]]). Jensen Huang, Nvidia's CEO, called it a mistake not to invest in Anthropic early, when Google and AWS did ([[2026-05-05-Amazons-Durability|Amazon's Durability]]).

## The journey

**2023: the shortage starts.** Because GPUs (the chips that train and run AI) were scarce, Amazon, Meta and Google began designing their own AI chips ([[2025-Gallaugher-Ch08-Amazon|Gallaugher ch.8]], p.298). Nvidia led training because it locked up high-bandwidth memory (very fast chip memory) before rivals and invested in links between chips ([[2026-05-11-The-Inference-Shift|The Inference Shift]]). In fiscal 2023 no single customer bought even 10 percent of Nvidia's sales ([[2026-09-13-Nvidias-Growing-Dependence-On-a-Few-Big-Customers|Nvidia's Few Big Customers]]).

**2025: power becomes the yardstick.** Because AI data centers run short of electricity, Huang argued at GTC 2025 that tokens per watt matters more than chip price ([[2026-05-05-Amazons-Durability|Amazon's Durability]]). (A token is a small chunk of text an AI reads or writes.) So Nvidia began pricing itself by the gigawatt: its sales chance per gigawatt grew from about $18 billion with Hopper to $25 billion with Blackwell and $40 billion with Vera Rubin ([[2026-09-01-Nvidia-Earnings-Dollars-Per-Gigawatt-Open-and-Hugging-Face|Nvidia Earnings, Aug]]). (A gigawatt is roughly the output of one large power plant.)

**February 2026: OpenAI doubles down.** OpenAI agreed to use an extra 5 gigawatts of Vera Rubin chips, 3 for running models and 2 for training ([[2026-02-27-What-Amazon-and-Microsoft-Will-Win-or-Lose-From-OpenAIs-New-Deals|OpenAI's New Deals]]). Nvidia's $30 billion investment in OpenAI appears to replace an earlier $100 billion plan that was never finalized ([[2026-02-27-What-Amazon-and-Microsoft-Will-Win-or-Lose-From-OpenAIs-New-Deals|OpenAI's New Deals]]).

**April 2026: a record quarter.** Thompson calls TSMC's (the chip factory's) new 3-nanometer plants "basically Rubin fabs" ([[2026-04-20-TSMC-Earnings-New-N3-Fabs-The-Nvidia-Ramp|TSMC Earnings]]). In the April quarter, sales hit $81.6 billion, up 85 percent in a year ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia Earnings, May]]). Net income was $58.3 billion, more than three times a year earlier ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia Earnings, May]]). (Net income is profit after all costs and taxes.)

**May 2026: agents bring Anthropic back.** Because agents (AI that does tasks, not just answers) use huge amounts of compute, Huang said demand had "gone parabolic" ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia Earnings, May]]). So Nvidia added Anthropic as a partner and lined up capacity for it on Azure, AWS and CoreWeave ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia Earnings, May]]).

**August 2026: growth set by supply.** Nvidia had grown 100 percent and forecast 70 percent growth for next year, far above the 45 percent analysts expected ([[2026-09-01-Nvidia-Earnings-Dollars-Per-Gigawatt-Open-and-Hugging-Face|Nvidia Earnings, Aug]]). Huang said demand is much greater than 70 percent, but supply caps what Nvidia can promise ([[2026-09-01-Nvidia-Earnings-Dollars-Per-Gigawatt-Open-and-Hugging-Face|Nvidia Earnings, Aug]]).

How the seller became a lender is in the [[journeys/nvidia-journey-late-2026|next era]].

## The rival: the customers' own chips

Nvidia's fiercest rivals are its own customers. Hyperscalers (the giant cloud firms) were about half of its data center revenue as of May 2026, and Thompson calls them "frenemies" because they most want to turn Nvidia into a plain chip maker ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia Earnings, May]]). Google and Amazon already use their own chip designs, and Microsoft, Meta and SpaceX are making theirs ([[2026-09-13-Nvidias-Growing-Dependence-On-a-Few-Big-Customers|Nvidia's Few Big Customers]]). In October 2026 Microsoft announced its Maia 300 chip and plans to deploy it at multi-gigawatt scale from 2027 ([[2026-10-13-Neocloud-Prime-Intellect-Acquires-Startup-To-Speed-Up-Inference|Prime Intellect Deal]]). In 2026 Google began selling its TPUs outright, not just renting them ([[2026-09-23-Google-Nears-Release-of-Flagship-Gemini-4-AI-Model|Gemini 4 Nears]]). Thompson argues Nvidia's CUDA software moat matters less than thought, since Anthropic and Google built leading models without it ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia Earnings, May]]).

Yet the two sides also converge. In August 2026 AWS said it would use more NVLink Fusion, Nvidia's chip-linking kit that it opened to other firms' chips ([[2026-09-16-Apple-Considers-Return-to-Server-Market-Has-Talked-With-Nvidia-to-Use-Network-Tech|Apple Server Talks]]).

## The idea behind it

- [[Custom-Silicon]]: big buyers design their own chips to escape Nvidia's prices ([[2025-Gallaugher-Ch08-Amazon|Gallaugher ch.8]], p.298).
- [[Dollars-Per-Gigawatt]]: Nvidia measures its market by power, not by chips ([[2026-09-01-Nvidia-Earnings-Dollars-Per-Gigawatt-Open-and-Hugging-Face|Nvidia Earnings, Aug]]).
- [[AI-Stack-Integration]]: once supply meets demand, most value goes to whoever integrates around a bottleneck ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia Earnings, May]]).

> [!warning] Misstep: missing Anthropic
> Google and AWS invested heavily in Anthropic early so it would use their compute, and Nvidia did not ([[2026-05-05-Amazons-Durability|Amazon's Durability]]). So Anthropic ran on TPUs and Trainium, and Nvidia's sales to it were "largely zero" until 2026 ([[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia Earnings, May]]).
>
> **Lesson (Huang's own):** he called not investing early a mistake ([[2026-05-05-Amazons-Durability|Amazon's Durability]]). Nvidia's 2026 deal spree, $30 billion in OpenAI alone, is that lesson applied ([[2026-10-07-Where-Nvidias-100-Billion-Dealmaking-Juggernaut-Will-Go-Next|Nvidia's Dealmaking]]).

## Three "why?" questions

<details><summary>Why are Nvidia's huge earnings "boring"?</summary>
Thompson argues sales are set by how many parts suppliers can make, so the numbers are predictable in a world short of chips ([[2026-09-01-Nvidia-Earnings-Dollars-Per-Gigawatt-Open-and-Hugging-Face|Nvidia Earnings, Aug]]).
</details>

<details><summary>Why does Nvidia price itself by the gigawatt?</summary>
Because AI data centers run short of electricity, Huang argued at GTC 2025 that tokens per watt matters more than chip price ([[2026-05-05-Amazons-Durability|Amazon's Durability]]).
</details>

<details><summary>Why can't the cloud giants simply drop Nvidia?</summary>
Thompson argues only hyperscalers and frontier labs are big enough to make it pay; in a fragmented world Nvidia wins ([[2026-09-01-Nvidia-Earnings-Dollars-Per-Gigawatt-Open-and-Hugging-Face|Nvidia Earnings, Aug]]).
</details>

## Sources

1. [[2025-Gallaugher-Ch08-Amazon|Gallaugher ch.8]] (FlatWorld, 2025).
2. [[2026-02-27-What-Amazon-and-Microsoft-Will-Win-or-Lose-From-OpenAIs-New-Deals|OpenAI's New Deals]] (The Information, 2026-02-27).
3. [[2026-04-20-TSMC-Earnings-New-N3-Fabs-The-Nvidia-Ramp|TSMC Earnings]] (Stratechery, 2026-04-20).
4. [[2026-05-05-Amazons-Durability|Amazon's Durability]] (Stratechery, 2026-05-05).
5. [[2026-05-11-The-Inference-Shift|The Inference Shift]] (Stratechery, 2026-05-11).
6. [[2026-05-26-Nvidia-Earnings-The-AI-Stack-Nvidias-New-Reporting|Nvidia Earnings, May]] (Stratechery, 2026-05-26).
7. [[2026-09-01-Nvidia-Earnings-Dollars-Per-Gigawatt-Open-and-Hugging-Face|Nvidia Earnings, Aug]] (Stratechery, 2026-09-01).
8. [[2026-09-13-Nvidias-Growing-Dependence-On-a-Few-Big-Customers|Nvidia's Few Big Customers]] (The Information, 2026-09-13).
9. [[2026-09-16-Apple-Considers-Return-to-Server-Market-Has-Talked-With-Nvidia-to-Use-Network-Tech|Apple Server Talks]] (The Information, 2026-09-16).
10. [[2026-09-23-Google-Nears-Release-of-Flagship-Gemini-4-AI-Model|Gemini 4 Nears]] (The Information, 2026-09-23).
11. [[2026-10-07-Where-Nvidias-100-Billion-Dealmaking-Juggernaut-Will-Go-Next|Nvidia's Dealmaking]] (The Information, 2026-10-07).
12. [[2026-10-13-Neocloud-Prime-Intellect-Acquires-Startup-To-Speed-Up-Inference|Prime Intellect Deal]] (The Information, 2026-10-13).

**Older than 2 years.** The "trillion-dollar" label and the start of in-house chips rest on the book's 2023 view.

**Where sources disagree.**
- Who Nvidia depends on: CFO Kress said in February 2026 the five biggest cloud firms were over half of data center revenue ([[2026-09-13-Nvidias-Growing-Dependence-On-a-Few-Big-Customers|Nvidia's Few Big Customers]]); Huang said in August that non-hyperscalers are about half and growing 100 percent a year ([[2026-09-01-Nvidia-Earnings-Dollars-Per-Gigawatt-Open-and-Hugging-Face|Nvidia Earnings, Aug]]).

See also: [[journeys/nvidia-journey|Nvidia journey (hub)]], [[journeys/nvidia-journey-late-2026|Nvidia, late 2026]], [[journeys/anthropic-journey|Anthropic journey]], [[journeys/openai-journey|OpenAI journey]], [[journeys/google-journey|Google journey]], [[Jensen-Huang]], [[Nvidia]].

## Change log

- 2026-10-13: Split from nvidia-journey.md per proposal 2026-10-13. Text moved unchanged; added the era intro, the era links and a third "why?" question from existing cited text.

<!-- claims: clm-48d13eca737e1740046c, clm-115a00f7f523e8b21978, clm-c0420d16b846c9f5b195, clm-34d07e2311799dbdd51a, clm-f505cbe2522b26c3a2f3, clm-4cd6b6eb00b099aa7d5a, clm-1e5d1b1096724f953371, clm-e098cd2e006eb74dd212, clm-201742be86edacc8f0b1, clm-73fc816544ee9e5af08d, clm-2773b6dafd62fe461c0c, clm-e1ca90a02f8e1fcca1c6, clm-586b27815a762bc12e52, clm-fcbd42125d3dac02d6d3, clm-ffce9acf754bf7911efc, clm-035fcc91e5a2f5df4cc1, clm-d6d049f7af6dbbef7640, clm-aa6010cf1b944097de3e, clm-22c8490997fb7940f00b, clm-9fa8a432ceca0f27f666, clm-43c49b2b15c0188856de, clm-98b0a2a99e507632b017, clm-c2d2d8d18f3f81d8aa1e, clm-ec4a08996f8ff7dc6781, clm-67d90a173da76eab9316, clm-0cf15556de2ac669fb95, clm-3caac4b6388d768085e1, clm-c98c4720cec919a6ef79, clm-db09efaa32d1cd7e313a, clm-f95e63c6993118c148a5, clm-eb2b80eacd90569f8604, clm-ac04bb04cbe7a08b9a3c -->
