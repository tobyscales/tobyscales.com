+++
authors = ["Toby Scales"]
title = "AI-Assisted Coding and the Disappearance of White Collar Jobs"
date = "2025-02-14"
description = "Not tryna freak you out, but you should probably definitely get a new job."
tags = [
    "predictions",
    "AI",
    "economics",
]
categories = [
]
+++
I spent the first part of this year coding with Gemini, and I thought I'd share my observations here because I believe my experience is a synecdoche of what's to come. 

First of all, I am someone who struggles with time and task management. Always have. I aspire to Inbox Zero, but I'm happy if I can maintain Inbox<50. So at the beginning of the year, while Google was performing its annual re-organization dance and my calendar was accordingly relatively light, I decided to invest in making some productivity improvements.

Perhaps because I struggle with time and task management, I'm always experimenting with new systems and methodologies for organizing my work and digital life. You could comb through my files and find a history of failed attempts to adopt [GTD](https://gettingthingsdone.com/), [Kanban boards](https://kanbantool.com/kanban-board) and [Zettelkasten](https://zettelkasten.de/overview/). All these attempts have run aground on the rocks of being not quite convenient enough, not available in the tool I want to or am forced to use, etc. Probably a familiar story to many lifehack-addicted corporate drones out there.

So in my spare time I thought I'd make a couple tweaks to a spreadsheet my team uses to track our customer meetings. First, let me say this: I am not a developer. Nor am I an Excel/Sheets jockey. But I do like automation, and I decided to crack open Google Apps Script to try to make my task-tracking spreadsheet talk to my Google Tasks list. After 3-4 hours of trial and error, staring at Apps Script documentation and how to make it run any time a cell in my "Follow Up" column changed, I was able to read a bit of data from my meeting tracker, then use that to create a new Task. Pretty nifty, I thought, and not bad for a day's work!

But then I got curious: could Gemini help me add a couple extra features? 

So I fired it up and *within seconds* I had the code I needed. I pasted it into my Google Sheet and everything worked a treat. Wow! That worked out so much better than I expected. But like any good developer, I wasn't satisfied. What if Gemini help me add a bit of natural langugage detection? Because ideally, instead of having to specify the exact date in my follow-up column I could just type "check in next week" and the automation would sort out when that should occur and schedule my Task accordingly. I asked the LLM, and it replied without hesitation. Again: fully working code, requiring little to no changes on my part. 

So began my descent into productivity madness. 

Since my Google Sheet-->Google Tasks automation was going so well, I wondered how hard it would be to add Google Calendar into the mix. Here, Gemini struggled a bit at first since Calendar doesn't provide the same extensibility that Docs/Sheets/Slides does; namely, you can't create custom UI elements for Calendar using Apps Script. You have to actually build a Workspace Add-On.

Again, **I am not a developer.** I would never undertake developing a custom Calendar add-on on my own, because it would be too challenging and time-consuming for me to learn all the nuances of Apps Script on top of resurrecting whatever bits of JavaScript I retain from the one course I took on it years ago. But with Gemini's help, I was able to develop a completely useful Calendar Add-On that allows me to tag all my Calendar entries using a dynamic list of tags that gets pulled from a Google Sheet. Specifically, I refer to our shared Customer List and use those names as tags for my Calendar entries, so I can track which customers I'm spending the most time with week-over-week.

Maybe this all sounds sort of "meh" to you, but here's what got me thinking.

Several years ago I was part-time CTO of an LA-based startup seeking to overhaul the wedding industry. We had big ambitions, but job #1 was to update the original codebase from the MVP and make it production-ready. So as I was re-architecting the infrastructure+code in advance of a v1 release, I relied on an Upwork dev team to help with shimming the existing code and adding a couple "Wow!" screens that would help us attract Series A investors. 

**This experience was exactly like my experience with Gemini.**

Iterative, conversational, with little tweaks here-and-there to nudge development in the right direction: "Could we make this button take up the full screen? Can we add a link to the privacy policy here?" That sort of thing. 

Which basically means that in the span of ~5 years, this type of entry-level software development went from offshored to basically free. _And that is going to be a big problem for a lot of industries._

LLMs are essentially data-distilling gateways slapped in front of mind-bogglingly large, loosely-structured datasets. Here are some examples of the datasets that LLMs will soon excel at distilling: medical journals, case law, and software code, state and federal regulations. Which professions do we currently trust to do that distilling? Doctors, lawyers, software engineers and judges. These are the jobs that LLMs will eat. 

And it's not going to happen slowly; it's going to happen very, very quickly.

We are on the cusp of a labor wipeout that will mirror the Industrial Revolution in terms of scale and impact, only instead of artisans being replaced with factories it's going to be knowledge workers replaced with AI. 

If your job, right now, is in any way to maintain a deep knowledge of obscurantist data -- get ready to be disrupted.

If your job is to translate from one language to another, even from deeply technical API specifications into plain English -- get ready to be disrupted.

Even for highly skilled salespeople and sales engineers, whose job can be roughly described as translating the output of one organization into a consumable, integrable package for consumption by another organization -- your job is going to be fundamentally different in the next 3-5 years, as AI will be capable of not only answering every deeply technical integration question your customers may have, but also interpreting the contract provisions, Terms of Service, et cetera. 

It will be nice at first; a highly capable assistant! One that has ready access to my domain knowledge! 

But make no mistake -- you will be training that assistant to take over your job one day. 

{{< figure src="/images/blog/escalated-quickly.gif" caption="Boy, that escalated quickly!">}}
