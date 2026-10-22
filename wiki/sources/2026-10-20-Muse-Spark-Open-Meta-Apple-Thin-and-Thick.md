---
type: source
title: "Muse Spark Open, Meta + Apple, Thin and Thick"
status: evergreen
created: 2026-10-21
updated: 2026-10-21
tags:
  - source
  - source/article
author: Ben Thompson
published: 2026-10-20
publisher: Stratechery
url: "https://stratechery.com/2026/muse-spark-open-meta-apple-thin-and-thick/"
raw: ".raw/captured/Muse Spark Open, Meta + Apple, Thin and Thick.md"
source_id: src-049bcd215b8fe390d6ed
---

# Muse Spark Open, Meta + Apple, Thin and Thick

Ben Thompson, Stratechery, published 2026-10-20.

## Summary

Meta released Muse Spark Open, an open-weight model optimized with Apple to run locally on high-end Macs using updated MLX software. Thompson analyzes the commercial restrictions on Meta's models compared to permissive Chinese models like DeepSeek and Qwen, noting that US labs face distillation constraints. Thompson attended a demonstration at Apple using two connected 512GB Mac Studios and argues local inference unlocks speculative branch-prediction coding workflows where tokens are effectively free, though high hardware costs and cloud scale keep thin-client architectures dominant for most workloads.

## Key claims

- Meta released Muse Spark Open, an open-weight AI model optimized to run locally on Mac computers, while Apple updated its MLX machine learning software toolkit to support it. (§ Muse Spark Open: “Meta Platforms said Thursday that it was releasing a new open-weight AI model and collaborating with Apple to run it locally on the company’s high-end Mac computers.”) ^clm-2f8a5e45d0380ba129c3
- Commercial services deploying Muse Spark Open must enter a formal agreement with Meta if their annual revenue surpasses $20 million. (§ Muse Spark Open: “Companies offering the model as a service must enter into a commercial agreement with Meta if their total annual revenue exceeds $20 million.”) ^clm-f9f87fb5b95478fda728
- Unlike Meta's license restrictions, Chinese models DeepSeek-V4.1-Flash and smaller Qwen models carry permissive MIT and Apache open source licenses. (§ Muse Spark Open: “both are effectively free to use as you wish.”) ^clm-897bcc23e5c952b1721a
- Thompson argues American open-weight developers suffer a disadvantage against Chinese labs because terms of service prohibit distilling frontier models, forcing US open models to distill distillations. (§ Muse Spark Open: “Because U.S. open weight model makers must follow the frontier labs’ terms of service, they (1) are worse than Chinese alternatives and (2) end up distilling the distillation”) ^clm-25bd6e5de0d9d4be48e6
- The United States Department of Homeland Security issued a directive ordering all federal civilian agencies to eliminate DeepSeek models from their IT environments. (§ Muse Spark Open: “Department of Homeland Security mandated that federal civilian agencies rid themselves of DeepSeek models”) ^clm-5dfcbb6dd1708df6a9f9
- Thompson notes that John Ternus replacing Tim Cook as Apple CEO helped thaw relations between Apple and Meta, enabling engineering collaboration on local AI. (§ Meta + Apple: “perhaps because of the replacement of Tim Cook with John Ternus as Apple CEO, there is an actual thawing of the relationship”) ^clm-d93b005ee59704b1cf33
- Apple demonstrated local AI development at its Cupertino campus using two Mac Studio computers with 512GB of unified memory connected via four Thunderbolt 5 cables. (§ Meta + Apple: “two Macs Studio with 512GB of unified memory linked together with four Thunderbolt 5 cables”) ^clm-e9f678d7c5678fdeeee0
- Thompson argues that running AI models locally creates effectively zero-cost tokens, enabling speculative coding where a harness builds multiple alternative feature paths overnight like CPU branch prediction. (§ Meta + Apple: “if inference is running locally, however, then you have effectively unlimited tokens, which means throwing away unused paths is costless”) ^clm-976af6d2c1c4935e1496
- Thompson maintains that thin-client cloud computing remains dominant because scarce high-end compute and massive memory aggregate most economically in centralized data centers. (§ Thin and Thick: “if compute isn’t yet good enough, then workloads will flow to wherever compute is the best, which is going to be in large data centers”) ^clm-ea6db657ad94343fbb37
- With high-spec 512GB Mac Studio rigs costing around $20,000, cloud API and subscription pricing remains more economically viable for the vast majority of users. (§ Thin and Thick: “Given that a reasonably equipped 512GB Mac Studio is probably going to be approaching $20,000 or so, even API costs”) ^clm-ef128dd3272ad4b11629

## Entities

[[Apple|Apple]], [[DeepSeek|DeepSeek]], [[John-Ternus|John Ternus]], [[Meta|Meta]], [[Qwen|Qwen]], [[Tim-Cook|Tim Cook]]

## Concepts

[[AI-Agents|AI Agents]], [[Distillation|Distillation (Training on Another Model's Outputs)]], [[Export-Controls|Chip Export Controls]], [[Local-Inference|Local Inference (Running AI Models on Your Own Hardware)]], [[Open-Weight-Models|Open-Weight Models]], [[Scale-Economies|Scale Economies]]
