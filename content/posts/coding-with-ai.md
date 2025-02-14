+++
authors = ["Toby Scales"]
title = "AI-Assisted Coding and the Disappearance of White Collar Jobs"
date = "2025-2-14"
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

Perhaps because I struggle with time and task management, I'm always experimenting with new systems and methodologies for organizing my work and digital life. You could comb through my files and find a history of failed attempts to adopt GTD, Zettelkasten, and Dewey's Organization Sheet. All these attempts have run aground on the rocks of being not quite convenient enough, not available in the tool I want to or am forced to use, etc. Again: probably a familiar story to many lifehack-addicted corporate drones out there.

So in my spare time I thought I'd make a couple tweaks to a spreadsheet my team uses to track our customer meetings. First, let me say this: I am not a developer. Nor am I an Excel/Sheets jockey. But I do like automation, and I know my way around the Formula Bar enough to (mostly) bend a spreadsheet to my will.

In my effort to automate away the more repetitive bits of my job, I decided to crack open Google Apps Script and try to make my task-tracking spreadsheet talk to my Google Tasks list. After 3-4 hours of trial and error, staring at Apps Script objects in the documentation and figuring out the "inner loop" required to code/test/run an Apps Script any time a cell changed, I was able to read a bit of data from a column on my task tracker, then use that to create a new Task. Pretty nifty, I thought, and not bad for a day's work!

But then I got curious: could Gemini help me add a couple extra features? Like: could it help me read data from a different column, and use that as the title of the Task? 

So I fired it up and asked the question. *Within seconds* I had the code I needed. I pasted it into my Google Sheet and everything worked a treat. Wow! That worked out so much better than I expected. But like any good developer, I wasn't satisfied. What if Gemini help me add a bit of natural langugage detection? Because ideally, instead of having to specify the exact date in my follow-up column I could just type "check in next week" and the automation would sort out when that should occur and schedule my Task accordingly.

I asked the LLM, and it replied without hesitation. Again: fully working code, requiring little to no changes on my part.

So began my descent into productivity madness. 

Since my Google Sheet-->Google Tasks automation was going so well, I wondered how hard it would be to add Google Calendar into the mix. Here, Gemini struggled a bit at first since Calendar doesn't provide the same extensibility that Docs/Sheets/Slides does; namely, you can't create custom UI elements for Calendar using Apps Script. You have to actually build an Add-On.

Again, **I am not a developer.** I would never undertake developing a custom Calendar add-on on my own, because it would be too challenging and time-consuming for me to learn all the nuances of Apps Script on top of resurrecting whatever bits of JavaScript I retain from the one course I took on it years ago. But with Gemini's help, I was able to develop a completely useful Calendar Add-On that allows me to tag all my Calendar entries using a dynamic list of tags that gets pulled from a Google Sheet. Specifically, I refer to our shared Customer List and use those names as tags for my Calendar entries, so I can track which customers I'm spending the most time with week-over-week.

OK, now here's where this gets scary.

Several years ago I was part-time CTO of an LA-based startup seeking to overhaul the wedding industry. We had big ambitions, but job #1 was to take over the slightly-dated codebase from an outsourced developer who had helped to build the MVP. As I was re-architecting the infrastructure+code in advance of a v1 release, I relied on an Upwork dev team to help with shimming the existing code and adding a couple "Wow!" screens that would help us attract Series A investors. 

**This experience was exactly like my experience with Gemini.**

Iterative, conversational, with little tweaks here-and-there to nudge development in the right direction: "Could we make this button take up the full screen? Can we add a link to the privacy policy here?" That sort of thing. 

So in the span of ~5 years, this type of entry-level software development went from offshored to basically free. _And that is going to be a big problem for a lot of industries._

LLMs are essentially data-refining gateways slapped in front of mind-bogglingly large, loosely-structured datasets. So 

