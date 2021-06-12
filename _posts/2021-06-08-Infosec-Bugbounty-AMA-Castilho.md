---
layout: post
title:  "Infosec Bugbounty AMA with Castilho"
categories: infosec-bugbounty-ama
excerpt : "AMA with Castilho"
author: Gurvinder Singh
---

# AMA with [Castilho](https://twitter.com/castilho101)

<br>

## CTF player for [@zh3r0__](https://twitter.com/zh3r0__) ⛳ | Bug Bounty Hunter 🐞

<br>

 - How do you overcome your stress and please suggest me a better way to grow in bug hunting with happiness and excitement I am very beginner and I just started my journey from a month ago?

   - ***I would say taking a break and keep your mind busy with something else.***

	- ***It’s been years since I started in this area and I still get excited with some things. If you really like this area, excitement and happiness will always be there.***

<br>

 - Q1) What are the common bug you get encounter in every other websites which is p1 or p2?

 - Q2) What is your recon strategy?

 - Q3) What learning resources do you follow in bug bounty?

   1. ***For sure, logic bugs that lead to ATO.***

	2. ***My recon strategy is basically subdomain enumeration, identify ports on each subdomain with rustscan + Nmap and fetch URLs on those subdomains with gau + use the tool reflection ( you can find it in my profile ). It's a basic strategy but works well for me.***

	3. ***Well, I read writeups that get disclosed and follow some big names in the industry ( check who I follow to get a better idea ), the basics really.***

<br>

 - Q1) Do you have checklist for approaching a target?

 - Q2) Resources for SSRF?

 - Q3) Approach to find senstive github secrets and credentials leak?

 - Q4) Race condition bugs methodology?

   1. ***I don't have a checklist but I do tend to learn much as possible about the target, by, for example, reading the documentation before playing the attacker role. By knowing the functionalities of your target, you will automatically create a checklist in your head saying " ok, this functionality seems like a good place to try for SSRF ", etc ... So yeah, it's very important before attacking a target, know your target and the checklist with come with that.***

	2. ***To get started with SSRF, I recommend <https://portswigger.net/web-security>, and to learn some new cool tricks, I recommend <https://book.hacktricks.xyz/pentesting-web/ssrf-server-side-request-forgery>. Oh, and reading CTF's or Bug bounty writeups about it. You can learn a lot by reading those.***

	3. ***For GitHub leaks, sometimes I use gitleaks but I tend to do that part more manually has automation can miss out on things. I recommend this video to learn some tips on how you can approach it manually - <https://www.youtube.com/watch?v=l0YsEk_59fQ>.***

	4. ***Usually for those kinds of bugs I just think about what could I duplicate and gain something out of it. For example, giving a like on a picture. You can potentially have 2 likes instead of one if vulnerable. Then, I just use turbo intruder <http://race.py> and wait.***

<br>

 - Do you follow any specific checklist for windows privesc? Can you share some good resources related to the same please?

   - ***I'm not very familiar with windows privesc, only did it once or twice in CTF's, but I do recommend <https://book.hacktricks.xyz/windows/windows-local-privilege-escalation>, that's where I found most of the info to privesc on those CTF's.***

<br>

 - Tips for mobile application pentest?

   - ***I’m mostly a web type of guy and never went very deep in mobile, but I would recommend the mobile section at hacker101 and trying to read the code of application really. It’s really easy to convert apk files back to the source code.***

<br>

 - Why bugbounty? What's your WHY?

   - ***Honestly, the reason I do bug bounties is the money. The possibility to merge a area that I love and make some money along the way is pretty cool.***

<br>

 - Being a CTF player, do you find instances where CTFs have relevance to bug bounties? Will playing CTFs increase my chances on finding bugs or they different?

   - ***I believe CTF's truly plays an important part in bug bounties. You are faced with the same challenge as a bug bounty program and that is to search for bugs. Also, CTF's are meant to put your skill into practice and improve yourself with some.***

	- ***New cool tricks you pick up along the way. So I would say, CTF's are important not only to solidify a new fresh topic but learn new stuff!***

<br>

 - CTFs generally have lots of section, like Forensics, Web App etc. Should I solely focus on Web Apps or learn it all to increase my chances on Web App bug bounties? Can you recommend some beginner resources for the same?

   - ***I mean, if you want to do bug bounties in the web section, just focus on the web section. There's no need to learn it all. To get started I usually recommend <https://portswigger.net/web-security> and reading writeups. You can learn a LOT by reading them!***

<br>

 - During bug hunting, what are the key things we should keep in mind?

   - ***Think that you're the first person testing the app.***

	- ***Try everything, even if it seems like a stupid idea.***

	- ***Take breaks, bug hunting can be mentally exhausting sometimes, and get back with a fresh mind.***

<br>

 - Any good resources where I can learn non known client or server side bugs?

   - ***Usually, to get started on a specific bug, I would recommend <https://portswigger.net/web-security>, that's what I use if I want to find out more about a client/server-side bug. Then, there's always some really clever, not very known, tricks with this bugs which I encounter when doing for example CTF's. So I would also really recommend reading some CTF's writeups from well-known CTF's. You can find them on <https://ctftime.org>.***

<br>

 - What does a good bug bounty report look like and what’s the process like for submitting it?

   - ***A good report is a report that provides a detailed description of where you've discovered the bug, how it can be exploited, and how the vulnerability works really. You can find some good reports and some tips in here: <https://docs.hackerone.com/hackers/quality-reports.html>.***

<br>

 - Can you tell about your first accepted report and the experience in Bug Bounty?

   - ***My first bounty / accepted report was when I was 18 years old. I reported a logic bug that lead to bypass a registration form, went to bed and woke up with a email saying my report got accepted. Needless to say I was pretty hyped after like 5 duplicates. Never give up.***

<br>

 - How do you decide the program/company to hack?

   - ***To be honest, first I see if the program pays bounties because I’m investing time into them, and then check if it’s a good scope of not. After I pick one, If I don’t find anything after 2 weeks (depending on the scope), I move on to the next one.***

<br>

 - How do you find that instinct where looking at a request or web page, it itself tells you "I am vulnerable"?

   - ***I would say that I would get an instinct if I saw, for example, an old-looking web page or that the target using a technology that the version is old really.***

<br>

 - What should new people start learning when starting in web hacking?

   - ***The basics really. How the internet works in general. Hacker101 has a great intro section for people that want to get started in this area and don’t know anything about it.***

<br>

 - How do you learn manual pentesting on web application?

   - ***To get started and learn new concepts I recommend <https://portswigger.net/web-security> and reading writeups. Then, solidify your new knowledge and learn even more with CTF's / challenges on burp academy and hacker101.***

<br>

 - When did you start hunting?

   - ***I got started in the cybersecurity area when I was 15/16. Throughout the years, I was doing small CTF's to learn new concepts and tricks + summer internships as a pentester on a company and, started doing bug bounties at 18 until now (I'm 20 at this minute).***

<br>

 - What do you do to overcome or avoid burnouts?

   - ***Taking breaks. Can't stress this enough. I usually go watch some youtube videos or go for a run or even take a shower (I occasionally find the solution for a problem while I'm taking a shower hahah).***

<br>

 - What is your favorite type of bug and why?

   - ***My favorite type of bugs are logic bugs. They can’t be found my automated tools and it’s fun to think irrationally when trying things out!***

<br>

 - Any specific resources for API security?

   - ***I recommend the following sources to learn about API pentesting:***

	  1. ***<https://book.hacktricks.xyz/pentesting/pentesting-web/web-api-pentesting>***

	  2. ***<https://www.youtube.com/watch?v=qqmyAxfGV9c>***

<br>

 - Q1) What is the most common vulnerability you personally encounter?

 - Q2) What got you into information security? How do you stay passionate?

   1. ***The most common vulnerability that I encounter is by far XSS, it's everywhere.***

	2. ***Honestly, I've always found it interesting how a person with a computer could have so much power in this modern times and eventually fall in love with this area.***

<br>

#### The original twitter AMA can be found here :- <https://twitter.com/sillydadddy/status/1402086843496112128> 
