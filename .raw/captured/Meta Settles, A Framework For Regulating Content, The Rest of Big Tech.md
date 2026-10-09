---
title: "Meta Settles, A Framework For Regulating Content, The Rest of Big Tech"
source: "https://stratechery.com/2026/meta-settles-a-framework-for-regulating-content-the-rest-of-big-tech/"
author:
published: 2026-08-31
created: 2026-09-09
description: "Meta’s settlement makes sense for all parties, but the entire sage highlights why any solution to regulating technology feels off."
tags:
  - "clippings"
---
**Listen to this post:**

Good morning,

On [Thursday’s episode of Sharp Tech](https://sharptech.fm/member/episode/metas-new-restrictions-for-teens-nvidias-open-source-investments-q-a-on-netflix-druckenmiller-parameters-and-performance), Andrew and I discuss Meta’s teen settlement, why Nvidia might be interested in Hugging Face, and why I don’t care that Stanley Druckenmiller used AI to write an op-ed in the Wall Street Journal.

On to the Update:

### Meta Settles

From [Bloomberg](https://www.bloomberg.com/news/articles/2026-08-26/meta-states-agree-to-settle-teen-social-media-harm-case):

> Meta Platforms Inc. said it agreed to pay up to $18 billion in landmark settlements to resolve social media claims from US states that would require the company to make major changes to how it operates platforms like Facebook and Instagram. Key parts of the deal, disclosed in a court filing Wednesday, require the company to put new guardrails on its platforms, including restricting how much time youths can scroll and preventing them from switching off certain safety settings without parental consent. The agreement includes payments to resolve a variety of claims across multiple lawsuits. At the heart of it was an ongoing trial in Oakland, California, in which multiple US states alleged that the company deliberately designed Facebook and Instagram to encourage compulsive use among young users.
> 
> Meta has agreed to pay up to $16.7 billion to resolve that lawsuit, according to the court filing. In addition, the company will pay another $459 million to resolve other privacy claims as well as $75 million in legal fees. Separately, Meta said it reached an agreement to pay Texas up to $1 billion. Some of the payments are contingent upon other social media companies adopting similar platform changes and making their own payouts. US District Judge Yvonne Gonzalez Rogers signed off on the agreement Wednesday after suspending the trial earlier in the day. In the earlier filing outlining the agreement, Meta denied the allegations against it and said the deal did not constitute an admission of liability.

There is certainly a discussion to be had about the issue of social media and children, fraught though it may be. The politics of it are pretty interesting, because I don’t think the topic breaks down on traditional partisan lines; rather, the more important cleavage is on what is usually considered the right, between conservatives and libertarians.

The latter are appalled at the prospect of the government, via the courts, dictating how people can use products; the fact a settlement does an end-run around First Amendment protections, resulting in de facto precedent (this settlement will almost certainly be used as the blueprint for others) about actively policing certain types of content, makes it even worse. The former, meanwhile, are more accommodating to government interference in private dealings in the pursuit of the common good, and one of the challenges facing Meta is the vague sense amongst nearly everyone that spending hours a day scrolling isn’t the best thing you can be doing with your life.

I will say I find myself very much torn on the matter. My son goes to a school where they have to put their phones in a lockable pouch that can’t be opened inside the school building, and I honestly think it’s pretty great, and has played a big role in how quickly he adjusted to living in America and made new friends. That’s maybe not directly analogous to this case, but I do recognize that it’s a lot easier as a parent to draw firm lines when the enforcement is completely out of your control; in this case, Meta blocking social media app notifications by default during school hours, and limiting usage otherwise, can be undone by parents, but defaults are powerful and easier to hold to.

At the same time, maybe parents should do their jobs? I say this feeling guilty about the amount of time my kids spend on their phones, but I also think it’s my responsibility as a parent, not Mark Zuckerberg’s and certainly not the government’s. The crux of this case, however, is that Meta is at fault, not because they enabled the posting of bad stuff — which would be shielded by Section 230 — but because they made product decisions that harmed children — haven’t you seen the rise in mental health issues amongst teens? And then I flip back to [this paper in NBER](https://www.nber.org/papers/w31493):

> Rising reports of suicidal behaviors in children and adolescents have led to the recognition of a youth mental health crisis. However, reported rates can be influenced by access to screening and changes in reporting conventions, as well as by changes in social stigma. Using data on all hospital visits in New Jersey from 2008-2019, we investigate two inflection points in adolescent suicide-related visits and show that a rise in 2012 followed changes in screening recommendations, while a sharp rise in 2016-2017 followed changes in the coding of suicidal ideation. Rates of other suicidal behaviors including self-harm, attempted suicides, and completed suicides were essentially flat over this period. These results suggest that underlying suicide-related behaviors among children, while alarmingly high, may not have risen as sharply as reported rates suggest. Hence, researchers should approach reported trends cautiously.

This obviously doesn’t tell the whole story, but it tells a part of the story that is often ignored in the rush to blame smartphones and social media for societal ills; and, at the same time, there’s the power of anecdata, and the sense that something is off — and the vector that is always the most politically potent is children.

### A Framework For Regulating Content

This brings me to Meta: the fact the company settled without an admission of liability is both understandable and also captures the dynamics of the case. Specifically, this was first and foremost a business decision, and a necessary one at that. The truth of the matter is that, from a business perspective, the entire previous section doesn’t matter. Meta was losing court cases, and faced the prospect of losing many more, at least until it could win at appeal, which was no guarantee.

The New York Times [wrote about how the settlement came together](https://www.nytimes.com/2026/08/29/technology/meta-states-settlement.html):

> For years, Meta, which owns Instagram and Facebook, seemed to have an impenetrable defense against child safety lawsuits. The company’s aces were Section 230 of the Communications Decency Act, a 1996 law that protects platforms from liability over what users post on their sites, and the First Amendment, which protects free speech. But concerns have mounted globally over the harmful effects of social media on children. Australia last year became the first country to bar children under 16 from using social media, and many other countries carried out or are considering similar rules.
> 
> In the United States, a flood of online child safety lawsuits have been filed since 2022, and the plaintiffs focused on a new argument claiming that social media sites designed their products in a harmful way that violates consumer protection and other laws. The suits accused the companies of knowingly creating sites that were as addictive as cigarettes, taking a page from a strategy used against Big Tobacco in the 1990s. Suddenly, relying on Section 230 didn’t look so safe. At Meta, concern was growing about the cases, according to two people familiar with thinking inside the company.

I do find the product safety argument compelling, insomuch as it aligns with my longstanding argument that there is a distinction worth drawing between what is posted and what is promoted by the algorithm. The attorneys general argue that Meta chooses to make the promotion mechanism addictive, and that that isn’t a free speech issue; I made a broadly similar argument in 2019’s [A Framework for Regulating Content on the Internet](https://stratechery.com/2019/a-regulatory-framework-for-the-internet/):

> How might society regulate content without infringing on rights or destroying competitive threats to the largest incumbents?
> 
> Start with this precept: the Internet ought to be available to anyone without any restriction. This means banning content blocking or throttling at the ISP level with regulation designed for the Internet. It also means that platform providers generally speaking should continue to not be liable for content posted on their services (platform providers include everything from AWS to Azure to shared hosts, and everything in-between); these platform providers can, though, choose to not host content suppliers they do not want to, whether because of their own corporate values or because they fear boycott from other customers.
> 
> I think, though, that platform providers that primarily monetize through advertising should be in their own category: as I noted above, because these platform providers separate monetization from content supply and consumption, there is no price or payment mechanism to incentivize them to be concerned with problematic content; in fact, the incentives of an advertising business drive them to focus on engagement, i.e. giving users what they want, no matter how noxious.
> 
> This distinct categorization is critical to developing regulation that actually addresses problems without adverse side effects. Australia, for example, has no need to be concerned about shared hosting sites, but rather Facebook and YouTube; similarly, Europe wants to rein in tech giants without — and I will give the E.U. the benefit of the doubt here — burdening small online businesses with massive amounts of red tape. And, from a theoretical perspective, the appropriate place for regulation is where there is market failure; constraining the application to that failure is what is so difficult.
> 
> The result is a regulatory framework that looks like this:
> 
> ![A drawing of The Regulatory Framework for the Internet](https://i0.wp.com/stratechery.com/wp-content/uploads/2019/04/Paper.stratechery-Year-One-copy.310.png?w=2000&ssl=1)
> 
> A drawing of The Regulatory Framework for the Internet
> 
> “Free as in speech” is guaranteed at the infrastructure level, the market polices platform providers generally (i.e. “free as in puppy”), while regulation is narrowly limited to businesses that are primarily monetized through advertising (i.e. “free as in beer”) and thus impervious to traditional content marketplace pressures.

I wrote this before COVID, which I found to be quite radicalizing in terms of the risks of even cracking the door to regulating content online, but I do stand by the overall framework. I would gladly trade Meta agreeing to restrictions on teens in exchange for a hardening of platform protections around free speech. Alas, that’s probably not how it’s going to play out, at least if Meta has anything to say about it.

### The Rest of Big Tech

From [Bloomberg](https://www.bloomberg.com/news/articles/2026-08-27/meta-s-pressure-campaign-puts-tiktok-youtube-snap-on-back-foot):

> Meta Platforms Inc. is mounting a public pressure campaign to make its social media rivals add guardrails to their platforms to curb teen usage, after signing a historic $18 billion settlement with US states requiring new safety features on Facebook and Instagram. The deal includes an unusual and significant incentive: a $5.3 billion portion of Meta’s payout over the next decade depends on whether its industry competitors commit to adding similar platform changes and agree to make comparable contributions to state initiatives to help kids. TikTok, Alphabet Inc.’s YouTube and Snap Inc. have so far stayed publicly silent. They have no legal obligation to make concessions, but legal experts and industry observers say the pressure from Meta and state attorneys general could force their hand.

This is where ripping off the bandaid doesn’t simply remove the legal overhang from Meta’s business, but also potentially helps Meta in the long run. First, from here on out — [starting with full-screen newspaper ads](https://www.bloomberg.com/news/articles/2026-08-28/meta-s-newspaper-ad-blitz-ups-pressure-on-social-media-rivals) — Meta is going to wear the cloak of child safety, doing everything possible to burnish its brand relative to its rivals. Second, Meta is going to leverage its relative utility to make TikTok look bad in particular, even as it seeks to diminish the undeniable educational benefits of YouTube. All things considered, I think Meta will consider it a win if TikTok ends up looking like the worst actor here.

Third, Meta isn’t sad about being mandated to ascertain the age of its users. The only way to do that effectively is to be that much more invasive in terms of collecting data, which is great for Meta; now they have the imprimatur of doing it for the kids. This also is where Apple is dragged into this: I have serious privacy concerns about age verification, but if it must be done I think that App Stores providing that verification is the best solution. The inescapable reality is that your smartphone provider is the single highest-trust relationship you have with technology: the operating system runs at root and reads everything, so a certain level of trust is already implied; given that, this is the right layer to know and certify your age.

But then again, why is that anyone’s business? This gets at why all of this feels so gross. Yes, there are issues with social media. And yes, technology makes it hard to be a kid, and hard to parent. Ultimately, however, where is the line between personal responsibility and accountability and the unrelenting march of bureaucrats — whether employed by big companies, the government, or the courts — dictating how we live, for our own good, of course (or for the children). Everything here makes sense, and I still kind of hate it.

---

This Update is also available as a podcast. To receive it in your podcast player, [visit Stratechery](https://stratechery.passport.online/member).

The Stratechery Update is intended for a single recipient, but occasional forwarding is totally fine! If you would like to order multiple subscriptions for your team with a group discount (minimum 5), please contact me directly.

Thanks for being a subscriber, and have a great day!