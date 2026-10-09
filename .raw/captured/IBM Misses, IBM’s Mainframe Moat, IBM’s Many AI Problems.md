---
title: "IBM Misses, IBM’s Mainframe Moat, IBM’s Many AI Problems"
source: "https://stratechery.com/2026/ibm-misses-ibms-mainframe-moat-ibms-many-ai-problems/"
author:
published: 2026-07-15
created: 2026-07-24
description: "IBM announced preliminary results that spooked the software market generally; this is a story, however, specifically about IBM and its mainframe franchise."
tags:
  - "clippings"
---
**Listen to this post:**

Good morning,

Summer is in full effect, which doesn’t just mean the summer schedule continues (i.e. no Stratechery Interview), but also NBA Summer League. Andrew and new Greatest of All Talk co-host Adam Mares discuss all of the new rookies and everything else happening in the NBA [in this week’s episode](https://goat.passport.online/member/episode/everyone-at-summer-league-is-thrilled-the-summer-of-second-apron-angst-how-to-be-an-nba-gm).

On to the Update:

### IBM Misses

From [Bloomberg](https://www.bloomberg.com/news/articles/2026-07-14/ibm-says-second-quarter-sales-missed-as-customers-pulled-back):

> International Business Machines Corp. shares slid the most in at least 58 years after the company reported preliminary second-quarter sales that fell short of expectations, attributing the miss to customers shifting their spending to chips and servers amid AI-fueled shortages. Preliminary second-quarter revenue totaled $17.2 billion, IBM said Tuesday in a statement, below analysts’ estimates of $17.9 billion. Sales from IBM’s infrastructure division, which includes mainframe computers, were especially hard hit, dropping 7%. The company said it’s still reviewing its books and final results, set to post next week, may be slightly different.
> 
> The shares plunged 25% to $217.07, the biggest single-day loss since at least Jan. 3, 1968, the earliest date for which Bloomberg has pricing data on the stock. IBM’s announcement initially weighed on other software companies, with stocks including ServiceNow Inc. and Workday Inc. slipping before making up some of the loss later in the trading day.

Software companies continue to, as Steven Tyler once sang, live on the edge: if one company reports something that reminds investors about software terminal risk in the age of AI, everyone plummets, deserved or not. And, in this case, I’m not entirely sure it was deserved; what happened to IBM was much more interesting, because hardware is always more interesting than software.

This filing from IBM was preliminary, which means there wasn’t an earnings call, just [a letter from CEO Arvind Krishna to investors](https://www.sec.gov/Archives/edgar/data/51143/000005114326000070/ibm-20260714xex991.htm). Here’s the key paragraph:

> When we discussed our expectations with you in April, we noted that we would be wrapping on the launch of z17 in the second quarter. Given this was the strongest start to a mainframe program in our history, we expected Infrastructure revenue to decline low-single digits for the year, beginning this quarter. What played out was worse than our expectations, driven by a shortfall in our Z performance and the associated software stack, primarily in Transaction Processing. In the last few weeks of June, we saw clients shift their quarterly capex spend toward servers, storage, and memory purchases to secure supply-constrained infrastructure ahead of expected price increases. This dynamic impacted client buying patterns. While we anticipated some supply chain related impact in our expectations, we did not anticipate the magnitude of the capex reprioritization. In addition, clients were distracted with rapidly-evolving, industry-wide cybersecurity concerns in the quarter.

This is a story that has very little to do with the ServiceNows and Workdays of the world, at least in the way that the market seemed to interpret it. Those companies — like all SaaS companies — sell products that are operational expenses for their customers, i.e. opex, not capex. That’s part of the entire premise of SaaS: you don’t need to make large up-front investments in your own software development and the hardware to run it on; you just pay a seat license every month.

The business Krishna is talking about is different: the z17 is IBM’s latest mainframe computer, and it costs real money to buy and install in the customer’s data center. That money is capex, not opex: you spend it up-front so that you can have the machine to use on an ongoing basis. What Krishna is saying is that some number of customers chose, at least last quarter, to allocate their budgeted capex numbers to non-mainframe servers, storage, and memory, crowding out IBM’s mainframe. And, to be clear, that’s a very plausible story — and it’s one that doesn’t have anything to do with crowding out of software licensing, which falls into the opex budget (a crowd-out could happen here as well, to be clear; it’s just more bureaucratically challenging than shifting capex budgets).

At the same time, there is a software story, as Krishna’s quote notes. Specifically, customers also pay IBM for the software that runs on those mainframes on an ongoing basis, which is opex. That opex, though, is very different from traditional SaaS: first, it’s intimately tied to hardware, and second, given that this hardware is used for Transaction Processing — think a massive retailer processing purchases, or an airline processing reservations — the pricing is much more akin to a usage-based model than it is a per-seat licensing model. That’s where the lack of upgrades stings: new systems create the capacity and contractual occasion for customers to add workloads and increase software consumption, and that expected expansion did not happen.

That noted, there is something that is curious about Krishna’s claims. Go back to [IBM’s Q3 2025 earnings call](https://seekingalpha.com/article/4832132-international-business-machines-corporation-ibm-q3-2025-earnings-call-transcript) and CFO Jim Kavanaugh’s prepared remarks:

> Transaction Processing revenue declined by 3%, reflecting another quarter of z17 outperformance as clients continue to prioritize hardware spend on our latest IBM Z system. While this dynamic impacts near-term revenue, we’re encouraged by a healthy pipeline that positions us well for future demand.

Krishna expanded on this point in the question-and-answer section of the call:

> Jim touched on Transaction Processing or mainframe software. We have seen this happen multiple times. In the first couple of quarters of a new cycle, TP tends to come down because people are very much focused on getting their hardware capacity. As that hardware capacity gets deployed, then the TP revenue begins to come up, along with some of the ELA cycle dynamics that are there, and we begin to see that. So I expect to see TP grow, not quite in double digits to be clear, but let’s call it low single digits, for sure, into next year.

So which is it? A year ago, when z17 sales were strong, IBM blamed those strong sales for lower-than-expected Transaction Processing software revenue. Now, when z17 sales missed, IBM is also blaming that miss for lower-than-expected Transaction Processing software revenue. Given that IBM stuck with the first narrative in the intervening two quarters — Transaction Processing grew, which IBM credited to those z17 sales — it sure seems to me that it’s this quarter that is the anomaly.

### IBM’s Mainframe Moat

One thing to notice about all of this discussion is the extent to which IBM manages to make money coming and going. SaaS companies may be an operational expense, but at least you don’t have to also pay for the servers the SaaS applications run on! With IBM, that’s exactly how it works: you pay capex for the hardware and opex to IBM for the software that runs on it. It’s an amazing business!

It’s also a business basically no one opts into, or has opted into for years. Any new company is going to build their infrastructure in the cloud; if they actually have a need for their own hardware, then they will buy the hardware and run Linux on it and write their own applications. It’s an opex versus capex trade-off; going with an IBM mainframe is choosing the worst of both worlds.

In other words, who IBM is selling to is existing customers, and those customers are trapped. Most of them have been IBM customers for decades. Again, think banks, airlines, etc.: these are entities that drove [the first wave of IT](https://stratechery.com/2024/enterprise-philosophy-and-the-first-wave-of-ai/), wiping out entire backrooms of bookkeepers in the process. They have gained the advantages of technology the longest of anyone; the price they pay is that their transactions are so numerous and complex that they can’t afford to move them, which leaves them at the mercy of IBM taking their pound of flesh.

At the same time, a move from mainframes can be done; United Airlines CEO Scott Kirby told me in [a Stratechery Interview](https://stratechery.com/2026/an-interview-with-united-ceo-scott-kirby-about-tech-transformation/):

> **SK:** We’re trying to do it all, because it all ties together. One of the big enablers was, that we started after I got here, we spent several hundred million dollars just getting off of our legacy mainframe systems, several hundred million rewriting code.
> 
> **Is that the key? That is the key enabler?**
> 
> **SK:** That was a key unlock. You can’t do what we do unless you do that first, it was a key unlock.
> 
> **So, just for the nerds, what was the system that you were running on before?**
> 
> **SK:** Oh, we were on, it was called SHARES, but it’s a Fortran-based system that was written in the ’60s.
> 
> **And so, what are you on now? Are you just on a regular cloud environment now?**
> 
> **SK:** We’re on our own stuff. Yeah, it’s all cloud and it’s our own stuff, but we spent hundreds of millions. It’s not done. In fact, the last cutover’s coming next year for the last piece.

[That upgrade was successful](https://www.paddleyourownkanoo.com/2026/02/04/united-airlines-is-in-the-midst-of-a-massive-tech-upgrade-that-has-taken-nearly-all-critical-services-offline-and-grounded-planes/), but Kirby may have overstated things: SHARES was historically run on Unisys mainframes operated by EDS and later HP, and the company [still has job listings for IBM mainframe developers](https://www.ziprecruiter.com/c/United-Airlines/Job/Mainframe-Developer/-in-Dallas%2CTX?jid=2945cb86508cf407). That noted, the job requirements are clear:

> Partner with modernization and cloud teams to support mainframe-to-cloud migration initiatives, including application inventory, dependency analysis, data extraction, and coexistence strategies with Java/Spring Boot APIs and Oracle data stores.

And:

> Contribute to system documentation, operational readiness, and decommissioning planning, supporting the transition from on-premises mainframe systems toward a modernized Azure-based cloud platform.

Now I’m not saying that IBM missed their numbers because of United; what I am saying is that:

- It is possible to move legacy businesses away from mainframes.
- Moving off a mainframe can eliminate IBM’s combined hardware-and-software tax and lower long-term marginal costs, although the migration itself may be extraordinarily expensive.
- United’s business has benefited significantly from its moves, because it enabled the airline to have the best tech stack in the industry, increasing loyalty amongst flyers like yours truly.

Still, who wants to actually do all of that work? It’s amazing United made that investment, but most companies will probably just pay IBM forever, because they don’t have the developers or budget to do the drudgerous work entailed in porting those mainframe applications to the cloud, which is a prerequisite for actually building new things.

But what if developers didn’t need to do it?

### IBM’s Many AI Problems

IBM’s short-term AI problem is exactly what happened this last quarter: mainframe customers repurposed spend that would have gone to upgrading their hardware to other hardware purchases, most likely to support their AI initiatives.

It’s the long-term problem, however, that is much more pernicious: of all the things that AI is well-suited for, porting code has to be near the top of the list. There isn’t any creativity or design involved, and you literally have a working example to compare output against. And what is the single most attractive code to port in terms of not just economics but also enabling innovation in your business? It’s the mainframe code; you can stop double-paying IBM on one side, and actually build on top of a modern platform on the other.

This, finally, gets at what I suspect started to happen to IBM this quarter, above-and-beyond the AI crowd-out: no, I don’t think that IBM customers suddenly ported their workloads off of mainframes. What happened is that IBM customers just became aware that it was possible to do so with AI. The way that translates for IBM’s business is twofold:

- First, if it’s now possible or becoming possible to move away from mainframes because of AI, then you don’t necessarily need to do it now, but you also probably don’t want to invest in a new mainframe. Best to limp along on what you have until you decide if a move away is feasible.
- Second, if it’s now possible or becoming possible to move away from mainframes because of AI, then it starts making sense to shift incremental usage somewhere other than mainframes; it certainly doesn’t make sense to re-up with IBM for bigger deals for more usage.

The optimistic outcome for IBM is that its customers ultimately decide that the risk of porting their most essential applications is not worth it, and they resume mainframe purchases and expand their software contracts. The pessimistic take is that they decide the opposite — and the longer they wait to decide without making any purchases, the better the AI will become!

It’s not all doom-and-gloom for IBM. Its consulting business grew, for example, thanks to companies looking for help in incorporating AI into their business. The company also framed Mythos as a positive in terms of driving their cybersecurity business. And, it should be noted, the company’s other hardware businesses benefited from that capex crowd-out. Still, I think the extremely high margin mainframe business is in trouble. Customers suddenly see a way out, and even if they stick around for now, it certainly behooves them to not pour more money into a product that once seemed inescapable.

---

This Update is also available as a podcast. To receive it in your podcast player, [visit Stratechery](https://stratechery.passport.online/member).

The Stratechery Update is intended for a single recipient, but occasional forwarding is totally fine! If you would like to order multiple subscriptions for your team with a group discount (minimum 5), please contact me directly.

Thanks for being a subscriber, and have a great day!