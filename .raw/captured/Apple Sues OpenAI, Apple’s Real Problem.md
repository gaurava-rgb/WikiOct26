---
title: "Apple Sues OpenAI, Apple’s Real Problem"
source: "https://stratechery.com/2026/apple-sues-openai-apples-real-problem/"
author:
published: 2026-07-13
created: 2026-07-24
description: "Apple is suing AI for stealing trade secrets; there is one guilty employee, but this mostly feels like lashing out."
tags:
  - "clippings"
---
**Listen to this post:**

Good morning,

On [last week’s episode of Sharp Tech](https://sharptech.fm/member/episode/meta-and-its-messaging-problem-the-xbox-reset-q-a-on-token-costs-american-soccer-starlink-in-nature), Andrew and I discussed Meta’s messaging problem, the Xbox reset, and why I’ve always been bearish on American soccer.

I am here on Monday with an Update: I couldn’t resist weighing in on the Apple-OpenAI lawsuit ASAP. I’ll be back two more times this week.

On to the Update:

### Apple Sues OpenAI

From the [Wall Street Journal](https://www.wsj.com/tech/apple-openai-lawsuit-f86bd58c):

> Apple sued OpenAI and one of its top executives Friday alleging the AI company stole trade secrets as part of its effort to develop competing devices. The federal suit filed in the Northern District of California accuses OpenAI’s chief hardware officer, Tang Tan, and Chang Liu, a member of its technical staff, of taking Apple’s confidential information through various methods. Both are former Apple employees who went to work for OpenAI.
> 
> The lawsuit shows how the relationship between the two companies has rapidly deteriorated since 2024, when they signed a deal to have OpenAI’s ChatGPT work with Apple’s Siri chatbot. Apple’s new Siri AI, announced in June, is powered by Google’s Gemini technology. Tan is leading OpenAI’s efforts to develop its own devices, a crucial strategic effort so that the company can reach consumers directly, rather than via other companies’ devices such as Apple’s iPhone…
> 
> Apple said in its suit that it lacks visibility into what OpenAI has done with its information but alleged that “at every level, from members of its Technical Staff to its Chief Hardware Officer, and in coordination with business partners, OpenAI has been stealing Apple’s trade secrets and confidential information.” A spokesperson for OpenAI said, “We have no interest in other companies’ trade secrets. We remain focused on building innovative technology that empowers people everywhere.” Tan and Liu couldn’t immediately be reached for comment.

You can read Apple’s filing [here](https://daringfireball.net/misc/2026/06/Apple_Inc._v._Chang_Liu_et_al.pdf), and almost everything you need to know is actually on the first page, in the first four paragraphs.

- Paragraph 1 is a succinct introduction to the case: “This case is about Apple’s former employees stealing Apple’s trade secrets for the benefit of OpenAI. Apple brings this suit to put a stop to it.”
- Paragraph 2 recounts how Apple has spent a lot of time and money building products that delight customers.
- Paragraph 3 basically says that everything they do is a trade secret.
- Paragraph 4 introduces one Chang Liu, and spends the next page-and-a-half recounting his crimes.

Liu is almost certainly guilty, and an idiot to boot. Apple has lots of details about Liu’s behavior, including downloading “dozens” of proprietary Apple hardware-related files and encouraging another Apple employee to do the same, because he did it on his Apple-issued laptop, and furthermore, logged onto Apple’s servers for weeks after he had already left the company.

A couple of quick points here:

- A few weeks ago there was a bit of a hubbub about [Meta capturing keystrokes](https://www.reuters.com/sustainability/boards-policy-regulation/meta-start-capturing-employee-mouse-movements-keystrokes-ai-training-data-2026-04-21/) from employees in order to train AI. What confused me was people’s surprise that a company had this level of access to company-issued hardware in the first place. Moreover, while that access may very well be theoretical for a lot of companies, at Apple it has always been a well-known fact — going at least as far back as when I was an intern there 16 years ago — that the company could and would go through everything if you ever crossed them.
- Apple’s security, as depicted in this case, is shockingly poor! First, the company lost track of the fact that Liu didn’t return one of his laptops, or disable it remotely. Second, due to what Apple claimed was a bug, Liu continued to have access to the company’s internal servers for weeks.

Regardless, Liu appears to be clearly guilty. I don’t think, however, that Liu is the point. What he is, from Apple’s perspective, is a fishing license. The company said as much towards the end of the introduction:

> This is the tip of the iceberg. Apple lacks visibility into what’s been happening behind closed doors at OpenAI, where such misconduct is normalized and exemplified by leadership. This much is clear, however: at every level, from members of its Technical Staff to its Chief Hardware Officer, and in coordination with business partners, OpenAI has been stealing Apple’s trade secrets and confidential information. As a natural result, OpenAI’s nascent hardware business now rests on the shakiest of foundations, rotten to its core by its illegal reliance on misappropriated trade secrets.

What follows are multiple appeals for discovery. Apple is actually only sure that Liu stole trade secrets; they want to use that proof — derived from their own laptop — to get access to everything OpenAI is doing.

### Apple’s Real Problem

The other named defendant in this case is Tang Tan, the former Vice President of Product Design for iPhone and Apple Watch, and almost every allegation Apple makes against him could easily be restated far more benignly: of course interviews touch on what employees have worked on — how would you know if you wanted to hire them otherwise? — and when it comes to the supplier allegation, [Patrick McGee wrote an entire book](https://stratechery.com/2025/an-interview-with-apple-in-china-author-patrick-mcgee/) about how Chinese suppliers take what Apple taught them and apply it to other products for other companies. I don’t think any of what is in the lawsuit is Tan’s — or OpenAI’s — real crime, at least in Apple’s eyes.

First, I think that Apple feels betrayed not just by Tan, but also Jony Ive. Start with the fact that [Ive framed his partnership with OpenAI](https://stratechery.com/2025/openai-acquires-io-openais-strategic-positioning-apples-worsening-ai-problem/) as an attempt to undo the harms he thought were caused by the smartphone, not exactly a ringing endorsement of the company that made him famous and rich. Apple can’t bring itself to attack Ive directly, which leaves Tan to bear the brunt of Apple’s fury.

Second, Tan is the point person for the four hundred people that Apple says that OpenAI has hired away from the smartphone maker. That is no crime, of course, although one gets the sense Apple sure thinks it is. From the lawsuit:

> Despite Apple’s rigorous security measures and practices, Apple’s trade secrets have been compromised through the deliberate misconduct by those previously entrusted with them. Apple’s former engineers and executives — recruited, directed and rewarded by OpenAI — along with OpenAI itself and its business cohorts, have been stealing Apple’s most sensitive information for a would-be competitor. With over four hundred former Apple employees now working at OpenAI, it is not surprising that certain OpenAI personnel have knowledge of Apple’s confidential and proprietary information, which they are obligated to keep confidential. But OpenAI has resorted to exploiting this confidential information, using it to extract still more from Apple’s current employees and trusted partners, and to structure its interview processes to try to solicit additional confidential Apple information—all while taking steps to conceal its actions. That OpenAI now employs people who were once entrusted with Apple’s trade secrets does not entitle OpenAI to use that information to jumpstart its hardware efforts.

That last sentence gets at one of the cruxes of the case: Apple’s trade secret claims in this case are impossibly broad; should this ever go to trial, narrowly defining what is and is not a trade secret will be a major point of contention. As it stands Apple is basically saying that any Apple employee at OpenAI is a walking trade secret, and, well, that’s why OpenAI hired them! From where else would OpenAI hire the personnel necessary to build a consumer electronics company?

That leads to a further point: Apple hasn’t really had competition for its best hardware and operations people until now. Yes, Meta had their headsets, and Google their phones, but from what I understand, there has never before been a mass exodus from Apple for a competitor like has happened in this case, and I don’t think Apple likes that very much! And Tan is the one leading the charge.

Third, just as Tan is the face of Apple betrayal, OpenAI is the face of AI generally, and it’s hard to escape the sense that Apple just really hates AI — and why shouldn’t they? Go back to 2022 and Apple had it all figured out: they had a lock on the premium end of the smartphone market, which they continued to slowly expand, even as they had figured out how to earn Services revenue from every iPhone user basically forever. Business was good!

AI has ruined all of that. Suddenly Apple had to make existential decisions about whether or not to compete in the model game, then they totally embarrassed themselves with the 2024 new Siri introduction, had their most prominent blogger declare that [Something Is Rotten in the State of Cupertino](https://daringfireball.net/2025/03/something_is_rotten_in_the_state_of_cupertino), had to completely overhaul their software and services teams, lost their position as kings of the supply chain and most favored customer of TSMC, to the point where they had to enact an emergency mid-cycle price raise, and then, worst of all, have to actually wrestle with the possibility that AI is such a paradigm shift that it actually might threaten the iPhone. And then, on top of all that, they lose 400 of their best employees — recruited by the lead hardware engineer for the iPhone, in partnership with their most famous executive outside of Steve Jobs — and have to know that all 400 of those employees are getting hit up by their former colleagues looking for a job as well!

The AI era has *sucked* for Apple. Even if they aren’t necessarily doomed, and even if the relaunched new Siri ends up working out, their position is still more fragile than it was, and everything about life is worse. Given that, how sweet it must feel to suddenly have a smoking gun in the form of a seriously dumb employee blatantly lifting documents, and to use it as a cudgel to exact revenge on the company that represents everything that is making your life miserable!

This perspective does make one wonder if that phrase “rotten to its core” was projection in the end. AI is changing the world, and Apple’s contribution is to deliver two year-old technology differentiated by exclusive access to data it won’t share. It certainly has no interest in delivering on a new AI-driven paradigm that endangers its iPhone franchise in any way; any of its employees who wish to do exactly that, meanwhile, are being told loud and clear that Apple doesn’t just think it owns your laptop, but also your mind and knowledge. I think it mostly stinks — but then again, rotten things usually do.

---

This Update is also available as a podcast. To receive it in your podcast player, [visit Stratechery](https://stratechery.passport.online/member).

The Stratechery Update is intended for a single recipient, but occasional forwarding is totally fine! If you would like to order multiple subscriptions for your team with a group discount (minimum 5), please contact me directly.

Thanks for being a subscriber, and have a great day!