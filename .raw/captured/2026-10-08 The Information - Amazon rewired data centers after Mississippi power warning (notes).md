---
title: "How Amazon Rewired Its Data Centers After Mississippi Power Warning"
author: Catherine Perloff
publication: The Information
published: 2026-10-08
url: https://www.theinformation.com/articles/amazon-rewired-data-centers-mississippi-power-warning
kind: reading-notes
note: "Paraphrased notes with short quotes, taken from Gaurav's subscription. Not the full article text."
---

# Notes: How Amazon Rewired Its Data Centers After Mississippi Power Warning

The Information, Catherine Perloff, 2026-10-08 (exclusive).

## The core story

- Earlier in 2026, Mississippi utility Entergy told Amazon it would have to start cutting the company's Mississippi data centers off the grid at peak times, so it could keep serving other customers (per two people with knowledge). This had not been reported before.
- AWS runs one data center near Jackson, Mississippi (being expanded) and is building two more facilities in the same area, which makes the state an important region in its buildout.
- The article frames it as a sign that AI power demand is pushing utilities to unprecedented measures; utilities rarely kick off major customers.
- In response, AWS changed the automated system that switches its data centers from the grid to backup power (such as gas generators). The new system is called **Project Falcon**. It lets the utility itself trigger the switch to backup power, without first contacting AWS (per one person).
- Project Falcon was built for Mississippi, but Amazon may use it elsewhere in the U.S. (per one person).
- Amazon says utilities in multiple regions can already remotely prompt it to use backup generation.

## Curtailment spreads across U.S. grids

- "Curtailment" means a utility tells a customer to cut power use or leave the grid entirely.
- Mike Sloan, CEO of power provider Synergetic: data centers are "pushing the capabilities of what the grid can do," so grid operators put special rules on them, and data centers must accept some curtailment.
- Texas: in 2025 the legislature passed a law letting grid operator ERCOT force large customers to curtail under certain conditions.
- North Carolina: Duke Energy added contract terms letting it cut large customers off the grid when needed (spokesperson).
- PJM, the largest U.S. grid operator (covers parts of Virginia and Illinois, among others), asked federal regulators for permission to cut large customers off first in emergencies, as part of measures to address a power capacity shortfall. It needs federal permission because its customers are utilities across several states.

## How other clouds handle it

- Google uses "demand response": shifting workloads to data centers in regions with spare electricity.
- In 2026 Google said it signed agreements with five utilities under this framework, committing to give up as much as 1 gigawatt of grid power when utilities need it elsewhere.

## Amazon's hunt for power

- Securing power has become one of the biggest bottlenecks of the AI data center buildout. AWS, described as the world's largest builder of data centers, pursues solar, batteries, nuclear and natural gas plants.
- End of September 2026: Constellation Energy said an Amazon deal would help fund a $3 billion, 190-megawatt expansion of its nuclear plant in Maryland; Constellation will also power Amazon data centers in the PJM region.
- Amazon's position: its buildout helps big companies finance new grid capacity (including in Mississippi) and gives utilities the certainty to invest in upgrades.
- Entergy Mississippi says it can require all customers to reduce grid use when demand exceeds supply, and that data center customers must install equipment to protect the grid from power quality problems caused by their large load.

## Backup power limits

- Federal rules limit diesel backup generators to 100 hours per generator per year outside emergencies.
- In 2025 the Minnesota Public Utilities Commission ruled against Amazon's plan to use 250 generators at a data center in Becker, Minnesota; Amazon abandoned that data center.
- Amazon says it runs backup generators minimally, mainly for testing and maintenance, and that state permits still apply regardless of utility arrangements.
- Batteries: Amazon has studied them as backup. Utilities worry about the grid load when batteries recharge. About a year and a half before publication, Amazon began talks with Dominion (Virginia) about battery backup; per one person, talks went nowhere because Dominion fears AWS charging at peak times. Amazon says it would never charge at peak; Dominion has been more risk-averse.
- Two years before publication, Amazon unveiled a battery system in Southern California that let solar-powered facilities, including data centers, keep running on carbon-free power after sunset. Its motive was sustainability, not AI power shortfalls.

## Owning the power plant

- Amazon bought a power plant in Pecos County, Texas, called **GW Ranch**, to power a nearby data center: its first data center fully off the grid (first reported by energy research firm Cleanview).
- GW Ranch's Texas permit allows emissions of 33 million tons of CO2, more than the largest U.S. coal plant, though Cleanview notes companies rarely emit their full permitted amount.
- Amazon also bought a solar farm and battery storage system in Oregon, which stays grid-connected (Cleanview CEO Michael Thomas).
- Thomas's point: before ChatGPT, siting a data center was standard (land, water, fiber, nearby power lines); now it is slower, harder and needs much more infrastructure.

## Why it matters for the wiki

- A new, concrete beat for the compute-scarcity story: the bottleneck is shifting from chips to grid power, and utilities now ration power to data centers.
- An Amazon journey beat: "build your own tools" extends to owning power plants (GW Ranch) and financing nuclear capacity (Constellation).
- A rival contrast: Amazon accepts curtailment with backup power (Project Falcon); Google moves workloads instead (demand response).
