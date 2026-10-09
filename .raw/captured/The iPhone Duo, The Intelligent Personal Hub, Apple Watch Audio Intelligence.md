---
title: "The iPhone Duo, The Intelligent Personal Hub, Apple Watch Audio Intelligence"
source: "https://stratechery.com/2026/the-iphone-duo-the-intelligent-personal-hub-apple-watch-audio-intelligence/"
author:
published: 2026-09-10
created: 2026-09-10
description: "Apple once again demonstrated the power of integrating hardware and software, but it’s biggest AI blindspot might be its belief in the primacy of apps."
tags:
  - "clippings"
---
**Listen to this post:**

Good morning,

John Gruber was at the iPhone announcement, and will discuss his first impressions of the iPhone Duo and everything else Apple announced on tomorrow’s episode of [Dithering](https://dithering.passport.online/member/).

On to the Update:

### The iPhone Duo

From [Bloomberg](https://www.bloomberg.com/news/articles/2026-09-09/apple-s-foldable-iphone-launch-event-gets-underway):

> Apple Inc. unveiled the company’s first foldable smartphone during a wide-ranging event Wednesday, betting that a new category can energize growth for its biggest-selling lineup. The device, called the iPhone Duo, will improve on rivals’ foldable models, newly appointed Chief Executive Officer John Ternus said, mocking competing handsets as “two phones awkwardly stuck together.”
> 
> The Duo unfolds to reveal a 7.6-inch (19.3-centimeter) screen, the largest display ever on an iPhone. There’s also an outer 5.4-inch screen for use when the phone is folded in half, and the device will be able to work with the iPad’s Apple Pencil stylus starting later this year. With the product expansion, Apple aims to show it can refine a category pioneered by Samsung Electronics Co. and other smartphone makers. The Duo is designed to have a sturdier feel, with less of a crease in the middle of the screen when unfolded. The software interface is also meant to capitalize on the new hardware and blend both screens together during use.

The iPhone Duo is very impressive, and very much Apple at its best (although I did laugh when the introductory video said “The convenience of iPhone Duo is combining the utility of two products into one”, given how Tim Cook once mocked the Surface for doing the same thing). The hardware engineering looks extremely impressive, but what is most noteworthy is how the company redesigned iOS to fit the device; that’s why Senior Vice President of Software Engineering Craig Federighi appeared in the introductory video:

<iframe title="VideoPress Video Player" aria-label="VideoPress Video Player" width="665" height="373.73" src="https://videopress.com/embed/ggjcoelQ?cover=1&amp;autoPlay=0&amp;controls=1&amp;loop=0&amp;muted=0&amp;persistVolume=1&amp;playsinline=0&amp;preloadContent=metadata&amp;useAverageColor=1&amp;hd=0" frameborder="0" allowfullscreen="" allow="clipboard-write; presentation"></iframe>

> We looked at every aspect of iOS to see how we could make it even more useful on iPhone Duo. Like you saw, essential controls are on the side to free up vertical space for content. This approach benefits your entire experience. For example, on the lock screen, it puts more focus. on your wallpaper, especially with this minimalist view that lets you really celebrate your favorite images, and we’ve brought this efficient use of space across the entire system, optimizing each of our apps specifically for iPhone Duo. The expansive display also supercharges productivity by letting you do more at once. You can move an app over to one side. and launch a second app on the other for powerful split-view multitasking, or launch a second window of the same app like Safari for comparison shopping with the same gesture you already know. Swapping apps is easy and so is changing sides and with a simple tap on the divider you compare the apps so it’s easy to to get back to them later. Using the large screen and portrait also feels great. If you’re multitasking while watching a video, you can pin it to the top from much larger view with plenty of space left below for your other app. As you can see, iPhone Duo is truly the most versatile iPhone ever, and we’ve taken it even further…
> 
> We’ve also made it easy for developers to adapt their apps for iPhone Duo with new and updated APIs. Zoom can turn the display into an immersive video conference room. You can easily see both the content being shared as well as the other participants on the call. Slack brings your whole workspace into view. The detail uses the new Core AI framework and runs its AI models on device to make content creation fast and easy on the big screen, and Netflix takes advantage of the versatility of iPhone Duo to make finding shows even more fun and engaging, scroll through clips on the outer display, or open up to get a captivating experience on the large screen. These are just some of the amazing apps being updated to take advantage of iPhone Duo and we can’t wait to see what developers are going to create.

My first complaint is personal: I am almost exclusively a left-handed iPhone user, so the dock being on the right is a no-go; I understand why Apple did it that way — that lets the dock stay consistent whether the Duo is open or closed, but if you only use one hand this is a right-handed device.

Second, it’s notable that Netflix was so prominently featured, particularly when you remember that Netflix [refused to support the Vision Pro](https://stratechery.com/2024/the-apple-vision-pros-missing-apps/). This is totally rational on Netflix’s part — Apple is going to sell a lot more Duos than they have Vision Pros — but it’s a reminder that app developers work with Apple purely out of self interest these days, not because they have any particular affection for the company.

The most notable thing that Federighi said, however, was the line about how Apple “made it easy for developers to adapt their apps for iPhone Duo with new and updated APIs.” Developers are going to need to put in effort to support the Duo, or they’re going to look terrible:

![](https://x.com/i/status/2097768433219690693)

Developers have been through this type of transition before, and modern apps built using Apple’s controls should adapt fairly easily, but they will need to do work; the iPhone is important enough that I expect most will.

### The Intelligent Personal Hub

That noted, the reason I highlight this aspect of the Duo is ultimately because of AI. Ternus spent a bit of time at the beginning of the presentation talking about the iPhone as the ideal AI device:

<iframe title="VideoPress Video Player" aria-label="VideoPress Video Player" width="665" height="373.73" src="https://videopress.com/embed/tqQuwIO7?cover=1&amp;autoPlay=0&amp;controls=1&amp;loop=0&amp;muted=0&amp;persistVolume=1&amp;playsinline=0&amp;preloadContent=metadata&amp;useAverageColor=1&amp;hd=0" frameborder="0" allowfullscreen="" allow="clipboard-write; presentation"></iframe>

> As we look ahead, we see a future filled with enormous discovery and transformation. AI makes entirely new kinds of experiences possible, and AI can become even more useful when it brings together your life, with the apps, services, and products you use every day. Then this means the product at the center of your experiences becomes even more essential, what I like to think of as an intelligent personal hub. It’s the intersection of broad new capability and a deep understanding of your personal context that makes this idea so powerful.
> 
> Now, If you were designing the ideal version of this hub from scratch, how would you do it? Well, first, you would want something that is always with you, deeply personal and able to bring intelligence to the moments when it matters most. You’d require a powerful processor that can run incredibly capable on device models to to quickly answer questions in the moment and pervasive networking access knowledge and even more capable models in the cloud. You need a large, beautiful display to show rich content. You’d add high-quality cameras and microphones, so you could see and hear and reason over the sights, sounds, and the world around you. Of course, you’d give it all day battery life. You’d want it to be super easy to use without a big learning curve, and finally, you’d want it to work seamlessly with your other devices, apps and services so it feels like one integrated experience. In other words, you would arrive at something remarkably familiar because there’s no product in the world better designed to be your intelligent personal hub than iPhone.

I don’t disagree about the intelligent personal hub framing; what is unsurprising is that Ternus’ description of what that intelligent personal hub should look like just happens to perfectly describe an iPhone. However, I’m not sure that makes it correct. For one, an iPhone, as powerful as it is, is just fundamentally less capable than something running in the cloud. Second, using powerful models for everything, as opposed to carefully rationed fall-backs to on-device models, is going to be more intelligent. Third, that all-day battery life would be tested if the intelligent personal hub were actually an agent that could do work even when you weren’t paying attention.

The obvious contrast is Meta’s Muse, which I think also fits the description of an intelligent personal hub. Muse runs in the cloud on a very capable dedicated VM, it uses Meta’s nearly state of the art models by default, and it can run continuously even when you aren’t interacting with it. That seems pretty compelling!

What is most interesting, however, is how the biggest advantage Apple has traditionally had may be a hindrance. There was a segment in the iPhone 18 Pro introduction highlighting Siri AI, and a couple of lines stood out to me:

<iframe title="VideoPress Video Player" aria-label="VideoPress Video Player" width="665" height="373.73" src="https://videopress.com/embed/coAw5mGm?cover=1&amp;autoPlay=0&amp;controls=1&amp;loop=0&amp;muted=0&amp;persistVolume=1&amp;playsinline=0&amp;preloadContent=metadata&amp;useAverageColor=1&amp;hd=0" frameborder="0" allowfullscreen="" allow="clipboard-write; presentation"></iframe>

> Siri can take action in the apps you already use including third-party apps like Stuff. Siri AI can find what you need and get more done than ever, and it already works seamlessly with over 300,000 apps. You can continue to take action in apps you already use with Siri, like texting a friend in WhatsApp, or playing a book on Audible, and it’s easy for developers to adopt new capabilities too. So you can ask Siri AI to draft an email in Outlook, search for a homework assignment in Notability, or add a restaurant recommendation to Tripsy…

To return to the Netflix point — and to the overall Apple frameworks advantage — it’s extremely impressive that Apple claims 300,000 apps work with Siri. Note, however, that the implication of it being “easy for developers to adopt new capabilities” is that developers have to actually put in the work — that’s work in addition to updating their UI for Duo.

In a world where everyone has to convince developers to build integrations, this wouldn’t be an issue. However, this is where browser use looms large: to the extent that agents can just use the web is the extent to which they get an integration with basically everything for free, and it’s Apple, with its dependency on developers plugging into APIs, who is at a disadvantage. Continuing with the same presenter:

<iframe title="VideoPress Video Player" aria-label="VideoPress Video Player" width="665" height="373.73" src="https://videopress.com/embed/9pK6niEd?cover=1&amp;autoPlay=0&amp;controls=1&amp;loop=0&amp;muted=0&amp;persistVolume=1&amp;playsinline=0&amp;preloadContent=metadata&amp;useAverageColor=1&amp;hd=0" frameborder="0" allowfullscreen="" allow="clipboard-write; presentation"></iframe>

> Beyond Siri AI, Apple Intelligence also boosts your productivity. In Safari, it powers Notify Me to monitor a webpage and automatically let you know about a change. In Shortcuts, you can make personalized automations just by describing them, like updating your calendar and reminders each time you receive an email from school, and in the phone app, Apple Intelligence can automatically surface relevant information when you call a business, like a a flight confirmation code right when you need it.

This is a subtler point, but perhaps the most profound: in Apple’s vision, the utility of Intelligence is defined by its ability to augment your existing workflow. Thus the reference to updating your calendar and reminders. It’s very possible, however, that the better workflow is to outsource a lot of work that used to happen in apps to the agent directly. What’s better, using a structured reminders app that you have to check, or simply being reminded directly by an agent? In truth the answer will likely vary by person, but it’s worth pointing out that Apple is so married to the app paradigm that they probably never even considered the alternative.

And so we’re back at Ternus’ introduction: he described an iPhone, but his vision assumes the primacy of apps; the truly Intelligent Personal Hub might not need apps at all.

### Apple Watch Audio Intelligence

John Gruber and I had a good discussion on [Tuesday’s episode of Dithering](https://dithering.passport.online/member/episode/agents-and-forklifts) about whether or not it was an issue that Apple was “late” to AI. It’s not always beneficial to be on the cutting edge, at least if you’re trying to reach normal users with a product they understand, and the actually functional Siri AI is likely to get a lot of usage. Indeed, you can make the case that the real problem with the initial Siri AI flop is that Apple announced it way too early out of a fear of being behind.

To that end, there was one feature Apple announced that made me uneasy. From [Bloomberg](https://www.bloomberg.com/news/articles/2026-09-09/apple-takes-on-ai-wearables-with-always-listening-watch-features):

> Apple Inc. is adding artificial intelligence-powered audio features and other new capabilities to its devices, including its premium smartwatch, to take on a growing category of AI wearables. The Apple Watch Series 12 and Ultra 4 models will have new Audio Intelligence tools, including Siri Recap, which uses ambient listening to take high-level notes of a wearer’s conversations throughout the day, Apple said Wednesday at its product event in Cupertino, California. There is also Live Recap, which shows a transcription of what was said in a live conversation in the last 15 seconds. The watch will also be able to listen to important sounds, such as a crying baby, doorbells and sirens.
> 
> Users can choose whether to opt into each new audio feature. Apple said no recordings will be created or stored by the new capabilities. Rather, the raw audio is not accessible to Apple and other apps and will be immediately deleted after processing.

There are wearables that do this and more, so Apple isn’t necessarily on the bleeding edge here; at the same time, the concept of wearable devices recording the real world makes me uneasy generally, and Apple rolling out that capability at scale means it’s going to be everywhere far more quickly than it would be otherwise.

It does appear that Apple has taken care with this feature, including not making raw transcripts available, even to the Apple Watch owner, but this is an area where I wish the company wasn’t early. Maybe surveillance by everyone you interact with is inevitable; I wish that Apple weren’t making it reality quite so quickly.

---

This Update is also available as a podcast. To receive it in your podcast player, [visit Stratechery](https://stratechery.passport.online/member).

The Stratechery Update is intended for a single recipient, but occasional forwarding is totally fine! If you would like to order multiple subscriptions for your team with a group discount (minimum 5), please contact me directly.

Thanks for being a subscriber, and have a great day!