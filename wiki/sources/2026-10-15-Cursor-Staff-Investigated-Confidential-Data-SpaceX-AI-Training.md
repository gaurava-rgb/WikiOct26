---
type: source
title: Cursor Staff Investigated Whether Confidential Data Reached SpaceX for AI Training
status: evergreen
created: 2026-10-15
updated: 2026-10-15
tags:
  - source
  - source/article
author: Grace Kay
published: 2026-10-15
publisher: The Information
url: "https://www.theinformation.com/articles/cursor-staff-investigated-whether-confidential-data-reached-spacex-ai-training"
raw: .raw/captured/2026-10-15 The Information - Cursor investigated confidential data sent to SpaceX (notes).md
source_id: src-5dce1df60966d968fdab
---

# Cursor Staff Investigated Whether Confidential Data Reached SpaceX for AI Training

Grace Kay, The Information, published 2026-10-15.

## Summary

Cursor engineers investigated whether internal testing of Grok Bot, code-named Sand, sent confidential customer, supplier, and partner records to SpaceX's AI unit for model training in late July 2026. A Cursor attorney warned that using the testing data could cause a major customer trust problem because the company lacked rights to train on enterprise data gathered across sales and recruiting. Cursor subsequently restricted access to corporate emails and barred employee data from model training. The episode followed earlier customer data leaks on Vercel marketing sites for Verizon, Bosch, and Coupa, as well as past security lapses at SpaceX and xAI.

## Key claims

- Cursor engineers investigated whether internal testing data containing confidential customer, supplier, and partner records was sent to SpaceX's AI unit for model training. (§ The core story: “Cursor engineers investigated whether internal testing data containing confidential customer, supplier, and partner information had been sent to SpaceX's AI unit”) ^clm-2adb640a521979010524
- The data investigation took place in late July 2026, weeks before SpaceX's AI unit publicly launched the Grok Bot autonomous personal agent. (§ The core story: “investigation occurred in late July 2026, weeks before SpaceX's AI unit (SpaceXSI) launched its Grok Bot autonomous personal agent”) ^clm-26a36ef1f3dbb424f4a8
- A Cursor attorney warned internal staff that using employee testing data to train AI models could trigger a major trust problem with enterprise customers. (§ The core story: “attorney warned employees in internal messages that using this testing data for training could trigger a major customer trust crisis”) ^clm-739d4d0abb6072986296
- A Cursor lawyer stated that broad use of Sand meant datasets contained confidential third-party details that the company arguably lacked legal rights to train on. (§ The core story: “lawyer noted that broad usage of the tool meant datasets included third-party confidential details that Cursor arguably had no legal right to use for model training”) ^clm-820ab47902fe54de9578
- Following the internal investigation, Cursor updated policies to exclude all employee usage data from future AI model training datasets. (§ The core story: “company changed policies to exclude employee usage data from future training datasets”) ^clm-262f0ba2df95ef9f5104
- Cursor led the development of Grok Bot, an always-on AI workplace assistant, to expand beyond coding tools into general enterprise workflows. (§ Grok Bot development and internal testing: “Cursor led the development of Grok Bot, an always-on AI workplace assistant intended to expand the startup's footprint into general enterprise workflows”) ^clm-81dceb348eaef1f5b702
- Cursor employees tested Sand across sales, recruiting, and research starting in June 2026, giving the autonomous agent access to internal databases and customer communications. (§ Grok Bot development and internal testing: “Staff members used the agent across departments including sales, technical recruiting, and market research, granting the tool autonomous access to corporate databases”) ^clm-669d171828cadb430c4d
- Several Cursor employees accessed Sand using personal email accounts, complicating company efforts to identify and remove their data from training pools. (§ Grok Bot development and internal testing: “employees accessed Sand using personal email accounts, which made it harder to trace and remove their data from training pools”) ^clm-32e0653da36689869691
- Earlier in 2026, Cursor sales and marketing staff inadvertently exposed confidential enterprise customer records through publicly accessible web pages deployed on Vercel. (§ Previous customer data leaks on marketing sites: “Cursor sales and marketing staff inadvertently leaked sensitive enterprise customer data through public websites deployed on Vercel”) ^clm-a55b8f08571ead3ae096
- An internal site for managing Verizon exposed managerial org charts, top users, email addresses, and software spending numbers embedded directly in readable front-end code. (§ Previous customer data leaks on marketing sites: “Verizon portal contained organizational charts of technical managers, lists of top Cursor users, user email addresses, and specific software spending figures”) ^clm-1b2c55bfd05a5a7fed86
- Cursor engineers responded to customer data exposures across client portals for Verizon, Bosch, and Coupa by creating an incident channel to take down the leaking sites. (§ Previous customer data leaks on marketing sites: “incident response channel titled "A ton of gtm sites that leak customer/internal data" to remove the exposed websites”) ^clm-1a7536a8fbbe49a78947
- In March 2025, a SpaceXSI employee exposed an internal Grok API key after accidentally uploading a test script to a public GitHub repository. (§ Security track record across SpaceX and xAI: “SpaceXSI employee exposed an internal Grok application programming interface key after accidentally uploading a test script to a public GitHub repository”) ^clm-8348b6ff93792bea7340
- In summer 2026, researcher discovery of Grok Build uploading entire Git repositories to Google Cloud storage led xAI to disable uploads and open source the tool. (§ Security track record across SpaceX and xAI: “researcher found that developer tool Grok Build uploaded entire Git code repositories to company Google Cloud storage buckets”) ^clm-2b9491f0c34fc99a05a2
- SpaceX completed its $60 billion acquisition of Cursor in mid-August 2026 to accelerate sales of enterprise AI products. (§ Security track record across SpaceX and xAI: “SpaceX completed its $60 billion acquisition of Cursor in mid-August 2026 to push into lucrative enterprise AI markets”) ^clm-88a6f62a2e347bc5510a

## Entities

[[Cursor|Cursor]], [[GitHub|GitHub]], [[Google-Cloud|Google Cloud]], [[Grok-Bot|Grok Bot]], [[SpaceX|SpaceX]], Vercel, [[Verizon|Verizon]], [[xAI|xAI]]

## Concepts

[[AI-Agents|AI Agents]], [[Zero-Data-Retention|Zero Data Retention]]
