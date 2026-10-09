---
type: entity
title: c-payne
status: developing
created: 2026-09-29
updated: 2026-10-09
tags:
  - entity
  - entity/company
claim_count: 4
---

# c-payne

Small independent maker of PCIe switches and adapters (c-payne.com) used to link GPUs directly in home AI rigs.

## Facts by source

### 2026-07-05 [[2026-07-05-jamesob-local-llm-Running-LLMs-Locally|jamesob/local-llm: Everything I know about running LLMs locally]]

- jamesob used PCIe Gen4 switches from indie maker c-payne so the GPUs can exchange data directly at wire speed, cutting latency without costly PCIe5 hardware. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-8fe7547a5cf7ed4c4f62|cite]])
- The c-payne PCIe switch parts cost about 1,220 euros, roughly $1,330. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-a26c6edcfb84160a25d5|cite]])
- With the switch working, jamesob measured GPU-to-GPU transfers of 27.5 GB/s one way and 50.4 GB/s both ways with under a microsecond of latency, the full Gen4 line rate. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-9d616957e40272661d68|cite]])
- A cheap-cable mistake cost jamesob time: an Amazon SAS cable that looked the same as c-payne's differed slightly and caused problems until he reordered. ([[2026-07-05-jamesob-local-llm-Running-LLMs-Locally#^clm-a1ce636f76fd4625e79a|cite]])

## Related concepts

[[Local-Inference|Local Inference (Running AI Models on Your Own Hardware)]]
