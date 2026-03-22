---
layout: post
title: "Separating the hype from the real in AI assisted development"
date: 2026-03-21
author: Matt
---

## The new paradigm hype cycle

For years, software engineering was in the dark ages. Projects were over budget, bloated, and missing the market. Then came the revolution that promised to change everything: It proposed an iterative approach to development that seemed modern and intuitive compared to old school top down waterfall style planning that it was attempting to replace. Of course, I'm talking about Agile!

Soon developers were advertising their Agile chops prominently on their resumes. Online courses offered "scrum master" certifications. Roles, teams, and even companies were adopting the "Agile" label. Books were written. Seminars were held. And so on.

The hype eventually died back, but agile itself never truly died. To this day, many of its core components: iterative development, sprints, and stand ups, continue to be practiced by engineering teams, even if they no longer use the "agile" label. Beneath the hype was a solid core of valuable ideas that stuck around.

The same story can be told about other tech trends: object oriented programming, functional programming, Java, UML, CASE. Each of these promised to revolutionize programming. They never fully lived up to their initial hype, but they also did contribute valuable ideas that have endured.

I think it is inevitable that AI assisted development follows the same path. Currently we are surely near the peak of the hype, and the promises are flying fast and thick. Some of these will fade away, others will stick. Let us attempt to untangle the hype from the real long term value.

## What's hype in AI assisted development

### Hype: AI means humans no longer need to own code

AI's ability to generate huge volumes of code has made human review and ownership of code a bottleneck. So, many people ask, why not take the human out of the loop altogether, and just allow the AI to write, review, and land the code all by itself? Maybe with a human observing from a distance. In this scenario, known as "human on the loop" (a cute way of saying "human not in the loop"), the human engineer is merely a manager of the AI, and the AI "owns" the actual code.

I think this practice is unlikely to endure, for the simple reason that human ownership is valuable to organizations. When something breaks, when a new feature is needed, it is valuable and useful to have a designated owner. Ownership also means accountability. Where there are business or legal risks in play, businesses need a person who can be accountable for outcomes. AI cannot play this role, only a human can.

When it comes to software, ownership and accountability require intimate knowledge of the code, and careful review of the changes that go into it. Businesses that value certainty and reliability (most of them) will eventually recognize this reality. Already, we are seeing signs of the limits of "human on the loop" in the form of [outages](https://www.techradar.com/pro/amazon-is-making-even-senior-engineers-get-code-signed-off-following-multiple-recent-outages) at Amazon and [data leaks](https://www.theguardian.com/technology/2026/mar/20/meta-ai-agents-instruction-causes-large-sensitive-data-leak-to-employees) at Meta. I expect that as time goes on there will be a broader recognition that "human on the loop" is hype that should be discarded.

### Hype: AI means the end of specialization, everyone is a "builder"

Some people such as Marc Andreessen have predicted that AI will cause traditional roles such as engineer, manager, and PM will all blur together, and everyone will become an "AI builder."

We should remember that Marc and people like him who make this claim are often working in startups, where there has always been blurriness between functions and roles, and AI no doubt increases this blurriness even further. However, it's a leap to assume that what applies to a startup also applies in larger organizations.

The assertion that AI makes specialization obsolete is usually made without elaboration. How it removes the need for non-engineering functions such as project management, people management, or design, is left unexplained. 

In fact, with engineering moving at a faster pace, it seems just as likely that AI could increase the need for these functions. The problem of how to organize resources, and the question of what to build and how to sequence it, the problems of people management, are more important than ever. These are problems that AI is less adept at solving compared to writing code. 

Given that code is now extremely cheap to write, what is gained by encouraging everyone to drop what they were doing and start writing it? This is hype.

### Hype: Token use, lines of code, or diff counts as a metric for impact

Counting lines of code has long been recognized as a bad metric for engineer productivity. With AI, this is even more so the case, as pumping out code is now effectively free. As has often been said, the question of what to build, taste and judgment are now where the value lies.

Yet many companies seem to be falling back onto bad habits these days, using token or code metrics as a proxy for productivity or AI adoption. It wasn't a good idea in the past and it isn't now.

## Looking for value beyond the hype

No one, least of all me, can deny that AI will have a profound impact on the software industry. The ways this will happen are too numerous to cover here. I'm going to talk about a couple that I think have been less often discussed.

### No hype: AI for prototyping

AI will have a profound impact on the way software is built, but there are subtleties to the picture that are often misunderstood. It is not the ability to write production code quickly that is most valuable, rather the most disruptive change comes from the ability of AI enabled fast prototyping to derisk product and technical decisions.

Up until recently, building software was an elaborate process largely designed around managing risk: the risk of building the wrong product, and the risk that the technical approach would fail. Because building software was expensive, a miss on either of these could lead to a lot of wasted resources.

To manage these risks, teams went through careful stages of planning and execution starting with gathering requirements, creating product vision, design, and technical roadmap documents, and carefully reviewing all of these before starting any work.

Execution was usually carried out in a phased approach that sought to validate core assumptions about the product and technical approach. Early validation of these assumptions was a way to manage the risk of spending a lot of time and resources on a dead end project.

AI's enablement of fast prototyping makes much of this process obsolete. Product and technical decisions can now be validated by building prototypes. Note that prototypes are distinct from product (aka production). Prototype code is not shipped to production and may be considered throwaway.

|  | Prototype | Product |
| :---- | :---- | :---- |
| **Goal** | Validate product and technical approaches | Build user facing software |
| **Priority** | Speed | Quality |
| **Risk** | Low: code is throwaway | High: code is pushed to users |
| **Who does it** | PM, design, eng | Mostly just engineers |

The prototype vs product distinction allows product designers, PMs, and engineers to optimize for speed when trying to validate product and engineering decisions, while keeping vibe coded slop out of the production code base. I think that in the future this distinction between prototype and product will become more widely recognized.

### Not hype: AI to improve product quality

We often hear AI talked about in terms of something that increases velocity but degrades quality by introducing "slop". However, this does not have to be the case.

AI is extraordinarily good at reviewing code, finding bugs, and writing tests. It can find performance regressions in automated tests, carry out automated bisects, and all of the other important but tedious work that h

As such, AI can be a powerful tool for increasing product quality, but this effect can be outweighed by bad practices such as "human on the loop" that allow low quality slop to enter the codebase without proper review. Eventually, businesses will have to decide how much they prioritize velocity vs quality. This is not a new tradeoff, but it becomes even sharper with AI.

## In conclusion

Comparing AI assisted development to previous trends such as Agile is a bit unfair. It's much bigger and more important than Agile ever was. Nonetheless, it is likely to follow the same basic pattern of hype, followed by a return to pragmatism. At this point, 16 weeks into this phenomenon, it is almost inconceivable that all of the common wisdom of today will be regarded as correct a year or two from now.

We should maintain a pragmatic mentality and be skeptical of bold revolutionary claims that are not backed up by sound reasoning, while looking for the long term value that the crowd may not yet see.
