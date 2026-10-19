---
title: "How DeepSeek Is Shaping Huawei’s AI Chips in a Growing Challenge to Nvidia"
author: Qianer Liu, Juro Osawa
publication: The Information
published: 2026-10-19
url: https://www.theinformation.com/articles/deepseek-shaping-huaweis-ai-chips-growing-challenge-nvidia
kind: reading-notes
note: "Paraphrased notes with short quotes, taken from Gaurav's subscription. Not the full article text."
---

# Notes: How DeepSeek Is Shaping Huawei’s AI Chips in a Growing Challenge to Nvidia

The Information, Qianer Liu and Juro Osawa, 2026-10-19 (exclusive).

## DeepSeek and Huawei engineering co-design

- DeepSeek is collaborating closely with Huawei Technologies to shape future AI chip designs, aiming to enable China to build frontier AI models without Nvidia hardware.
- Huawei engineers have been stationed at DeepSeek offices for extended periods to incorporate DeepSeek requirements on calculations and inter-processor data movement for chips debuting in 2027 and beyond.
- The collaboration represents a unified effort on an issue central to Beijing technology policy, which limits Nvidia purchases by domestic firms.
- Nvidia chief executive Jensen Huang stated in May 2026 that Nvidia had largely conceded the Chinese AI chip market to domestic competitors.
- DeepSeek plans to begin using Huawei current flagship Ascend 950DT chip for pre-training models as early as the end of 2026.
- Huawei plans to allocate most of the initial supply of its next-generation Ascend 960DT training chip to DeepSeek when it releases in the first quarter of 2027, rather than distributing it broadly across China.
- Huawei announced an annual release cadence for Ascend processors: Ascend 960DT in the first quarter of 2027, Ascend 970 in 2028, and Ascend 980 in 2029.

## Performance gap and covert access to Nvidia Blackwell

- Research institute Epoch AI estimates that Nvidia B300 chips deliver approximately seven times the raw arithmetic performance of Huawei Ascend 950.
- Epoch AI projects Huawei will remain three to four years behind Nvidia on single-chip performance through 2030.
- United States export restrictions since 2020 barred Huawei from Taiwan Semiconductor Manufacturing Co (TSMC) fabrication and limited access to advanced high-bandwidth memory (HBM).
- Despite committing to Huawei chips, DeepSeek continues seeking Nvidia advanced Blackwell chips.
- DeepSeek obtained barred Blackwell chips via intermediaries who purchased servers in permitted countries, set them up in inspected data centers, disassembled them, and shipped the chips into China to train DeepSeek V4 models.

## Breaking CUDA lock-in with TileLang

- DeepSeek is bypassing Nvidia CUDA software lock-in using TileLang, an open-source programming language developed by Peking University researchers and released in January 2025.
- TileLang allows engineers to write compact kernel programs that execute AI calculations across different hardware architectures without starting from scratch.
- DeepSeek used TileLang for its V4 models and recently released a TileLang version tailored for Huawei Ascend 950 chips with five code suites covering necessary calculations and data transfers.
- DeepSeek stated Huawei engineers gave unreserved assistance in adapting TileLang to Ascend hardware.
- Huawei is assembling supernodes of Ascend 950DT chips at volume; Rotating Chairman Eric Xu stated training tests went well and expects widespread adoption by 2027 while domestic supply remains constrained.
- Full pre-training of a frontier model requires well over 10,000 Ascend 950DT processors running uninterrupted for weeks.

## Why it matters for the wiki

- AI shift story: shows how software compilers like TileLang erode CUDA lock-in, enabling model developers to move workloads across chip vendors.
- China AI race and export controls: demonstrates how Chinese labs navigate sanctions through domestic co-design (Huawei) while smuggling frontier Blackwell silicon for top-tier training.
- Nvidia journey: confirms domestic Chinese erosion where Nvidia lost control of domestic frontier training clusters.
- Huawei journey: details Huawei annual Ascend silicon roadmap (960DT, 970, 980) and deep hardware-software integration with DeepSeek.
