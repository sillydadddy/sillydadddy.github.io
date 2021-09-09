---
layout: post
title:  "Infosec Bugbounty AMA with MorningStar"
categories: infosec-bugbounty-ama
excerpt : "AMA with MorningStar"
author: Gurvinder Singh
---

# AMA with [MorningStar](https://twitter.com/0xMstar)

<br>

## Bug Bounty Hunter at [@BugCrowd](http://www.bugcrowd.com) 🐞

<br>

 - How can we get our first bug. How to choose targets and how a beginner should approach it?

   - ***Getting first bug is lot easier now just run nuclei on all bugbounty target you will get many but probably dupe. Choose target with large scope as beginner & look for common bugs like rxss which hard to prevent & easy to find & mostly everywhere.***

<br>

 - Q1. If you had to restart your journey, what bug you will be focusing on first?

 - Q2. What you focus on when you pick a target?

 - Q3. What your favourite bug you found?

 - Q4. What bug you took time to escalate or get?

 - Q5. Any future plans of [@PrettyRecon](https://twitter.com/PrettyRecon)?

   1. ***XSS.***

	2. ***I focus on IDOR & rpiv escalation, sometimes XSS, depends upon tech stack.***

	3. ***Super admin account takeover.***

	4. ***XSS & privileged escalation.***

	5. ***Support can tell you more, I do not spend much time in development now, they were planning to build search engine for cloud.***

<br>

 - What are the most common bugs you reported on Bugcrowd?

   - ***Mostly XSS , IDOR, privileged escalation, information disclosure.***

<br>

 - Why you hack?

   - ***Money mostly but after one perticular target I hunt for competition.***

<br>

 - Which burp extension do you use?

   - ***I always use community version of burpsuite, recently purchased burp pro, only use this two mostly.***

<br>

 - Do you take notes when you hack, if yes which tools or app do you use?

   - ***I actually do, but in a very inefficient way. I use notepad++.***

<br>

 - Your focus is more on privelege escalation bugs so do you use extensions like autorepeater or autorize? If yes, any tips on getting the most of this tools.

   - ***Yup start with reading docs if program is relatively old & learn how user roles are, which permission they have then list down endpoints which are accessible fo high priv users try to visit them from low privileged account, play with request url, request type etc.***

	- ***Try to access functions which are not accessible without confirming email or phone number.***

	- ***I used Autorize before but manually finding for those bugs is always better otherwise you will miss a lot of things.***

<br>

 - What tasks do you automate? Do you have new endpoints alerts? What are the most reported P1s?

   - ***I automate subdomain finding & running nuclei on new targets with custom templates. I do not have new endpoint alert system. I usually focus on same programs again & again so if I found anything new in Ui then I test that feature.***

<br>

 - What you feel when your report gets closed as duplicate of internal finding or you don't get rewarded as you deserve?

   - ***Obviously gets frustrated, but I usually move on from that program & never hunt on them.***

<br>

 - How do you manage your time?

   - ***It's hard man, sometimes I spend unhealthy amount of time infront on machine & that's not good.***

<br>

 - What are the most useful tools for you?

   - ***Project discovery have some awesome tools other that than I use some paid tools.***

<br>

 - How do you test xss, and csrf with burp community, any extension for burp community that can save my time?

   - ***I mostly hunt those bug manually, I only use secret finder & linkfinder.***

<br>

 - Can you shares some resources on IDOR, Priv Escalation and Information Disclosure?

   - ***I personally do not find any good resources, H1 hacktivity is good start, also check reconless YouTube channel.***

<br>

 - What is the first bug you try to look for when you start?

   - ***IDOR, privlege escalation.***

<br>

 - How to approach any target?

   - ***Depends on type of target, if large scope wildcard then I usually run [@PrettyRecon](https://twitter.com/PrettyRecon) first as it gives you basic data to further analysis & sometimes low hanging fruits of target is relatively new. After that I logged in main app & browse full website as a end user.***

	- ***Keeping burp proxy on & then just play with requests, also spend hours reading there support/help/documentation pages.***

<br>

 - How long did it take you to become a professional bug hunter?

   - ***I still do this part-time, doing it from last 3-4 years may be, may be more.***

<br>

 - How much time do you spend hunting bugs?

   - ***Daily 2-3 hours & rest full weekend.***

<br>

 - How to improve in web bug hunting?

   - ***Automate wherever possible, learn new techniques & try to implement same in code. Solve labs portswigger, pentester lab etc. Spend money in learning & buying service tools(this I learn recently).***

<br>

 - Where you found most bug means private program or public?

   - ***Private, been while since I hunt on public program.***

<br>

 - What are your most targets means small scope with more functionality or large scope or where you spend more time in recon/automation or manual?

   - ***Small scope with lots of functionalities. I do Recon & automtion buy most of time I spend manual.***

<br>

 - How to do manual recon or how you perform manual recon? What are the things keep in mind when you doing manual recon?

   - ***Recon thing must be automated doing it manually is very inefficient & I made that mistake before but actually you can write simple bash script to automate lots of things or iron source tools are also available. Manually running same commands again & again in waste of time.***

<br>

 - How do you choose your program and what motivate you to keep hunt on it for more than month?

   - ***I checked tech stack first, I have web development experience so if target using same tech stack I target them first as I know where can they misconf something.***

	- ***Reward, fast triage & fast resolve only keep me motivated to spend on one target.***

<br>

#### The original twitter AMA can be found here :- <https://twitter.com/sillydadddy/status/1431913857010728963>
