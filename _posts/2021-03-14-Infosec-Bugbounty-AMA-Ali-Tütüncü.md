---
layout: post
title:  "Infosec Bugbounty AMA with Ali Tütüncü"
categories: infosec-bugbounty-ama
excerpt : "AMA with Ali Tütüncü"
author: Gurvinder Singh
---

# AMA with [Ali Tütüncü](https://twitter.com/alicanact60)

<br>

 - How old have you been doing this? Can you recommend resources for beginners?

   - ***I'm doing this since 18. I started to bug bounty in 2016.***

   - ***Here are some resources for beginners:*** 

     - ***<https://pentester.land/list-of-bug-bounty-writeups.html>***
	 
	 - ***<https://hackerone.com/hacktivity>***
	 
	 - ***<https://google.com/search?q=bug+bounty+writeups&oq=bug+bounty+writeups>***

<br>

 - Your methodology to hunt and what tools do you use?

   - ***I start my test with subdomains. Register > try account takeover > search csrf vuln on important requests > search xss issues > search IDOR issues etc. It depends on the target.***

   - ***I use some classic tools like burp suite, amass, gau, sqlmap, arjun, ffuf etc.***

<br>

 - Did you ever feel like you’re stuck and cant learn or do something about BB? If you did, what did you do?

   - ***Actually, I always feel that because I don't have technical information about vulnerability types. I can find XSS vulnerability but I can't fix it. Hmm, I guess nothing. I just trying to improve myself.***

<br>

 - Please share with me your recon structure? How do you analyze your hunting on a program you just got invited, I’ve seen you on some programs you never and some of them alot is there anything that interests you in that specific program?

   - ***Actually, I'm not a recon guy. I list all subdomains and start testing. I try to broke my target's features and then search for technical vulnerabilities. The main thing that I do is understanding my target. I read all docs that about my target so I can understand how to attack.***

<br>

 - Q1. When did you started learning about hacking with 0 knowledge?
 
 - Q2. How did you become so good in very less time?

 - Q3. Any tips for beginners like me?

     1. ***I started learning about hacking at 2016.***

     2. ***I think i'm not good, yet. But I guess I watched all poc videos & read all writeups and disclosed reports to earn these achievements. For example, I register to the website and see Webhooks feature.***

     3. ***I remember a writeup I read before so I already know how to attack there.***

<br>

 - Any weird bug you reported which you are proud of? Your favourite public program? Are you using laptop?

   - ***I reported an Account takeover vulnerability. I registered with the existing email and takeovered the victim's account.***

   - ***My favorite public program is Verizon Media.***

   - ***I use a notebook (Monster Abra A5 v13.3.1, it's a Turkish company) but I bought a desktop last week.***

<br>

 - How much time the hardest bug you found took for you to exploit?

   - ***Hmm, actually I don't remember it but some XSS wafs are really challenging and funny.***

<br>

 - Q1. Which learning materials(blogs, books, courses, tutorials) and labs do you utilise to sharpen your skillset?

 - Q2. Give me a brief about your Bug Bounty Setup(toolings, methodology/checklist, note-keeping, VPS etc).

   - ***All writeups & disclosed reports, [@Bugcrowd](https://twitter.com/Bugcrowd)'s contents, [@WebSecAcademy](https://twitter.com/WebSecAcademy)'s labs. Also, [@NahamSec](https://twitter.com/NahamSec)'s streams & [@Farah_Hawaa](https://twitter.com/Farah_Hawaa)'s videos are very helpful for hackers.***

   - ***I don't have a big setup. I use classic things like burp suite, sqlmap, gau etc.***

<br>

 - Whats your methodology when you open up a new target?

   - ***I start my test with subdomains. Register > try account takeover > search csrf vuln on important requests > search xss issues > search IDOR issues etc. It depends on the target.***

<br>

 - How do you motivate yourself when you get duplicates or something bad? How to keep yourself in hacking mode?

   - ***I set a goal for myself and try to achieve it. That motivates me. My closest goal is being in TOP10.***

   - ***Actually it depends on my mood. If I feel good, I can search for bugs all day without getting bored.***

<br>

 - Do you use cwel? How do you build your word lists? Or do you just use the ones from Jason Haddix or some other ready-made list available on the internet?

   - ***I don't use cwel (and don't know what's it). I use ready-made wordlist (especially [@DanielMiessler](https://twitter.com/DanielMiessler)'s wordlists).***

<br>

 - What the first things you do in a limited scope? Manual or automation?

   - ***I register to the website and try to understand the logic of the site. For example if it's a shop company, I try to access other users' orders or address information. Then try to search classic things like csrf, xss, ATO etc.***

   - ***I would try to search vulnerabilities that don't require authentication like rxss. If can't find, I would leave the program.***

<br>

 - Which vulnerabilties you hunt? How you find 15 or 20 bug in a month? When you start hunting as beginner how much time you give on program?

   - ***I don't have specific bug types but I have favorites like xss, information disclosure, business logical errors etc.***

   - ***I'm full time bug hunter. It's my job.***

   - ***4 years ago I started bug bounty.***

   - ***It depends on the target. If it has a big scope, I can hunt there all time.***

<br>

 - Your methodology for SSRF?

   - ***To be honest, i'm not a ssrf professional. I try it on classic features like webhooks. Firstly I try to get ping using ngrok. If my target hit me, I try to improve the impact.***

<br>

 - How many hours do you spend hunting in a day?

   - ***It depends on my mood. If I feel good, I do it all day. If I feel lazy, I don't hunt. I wait to feel good. These days I hunt 7-8 hours a day.***

<br>

 - Which programs will you suggest beginners to hunt?

   - ***ATT & Microsoft. Actually I suggest all programs whose scope is big.***

<br>

 - Top 5 tools that you use?

   - ***Burp Suite***

   - ***Gau***

   - ***Ffuf***

   - ***Sqlmap***

   - ***JsLinkFinder (Burp Extension)***

<br>

 - Do you stick to every invite/program you get invited or picky about what kind application you want to hack, I feel like I'm too picky about my targets?

   - ***If I like my target or enjoy, I test them. I have a few company types that I don't like such as crypto companies.***

<br>

 - What are the 3 types of bugs that you report the most?

   - ***Privilege Escalation***

   - ***XSS***

   - ***Information Disclosure***

<br>

 - How do you pick your target?

   - ***I like programs that pay good money and have big scope. It's not big deal if the program is old or not.***

<br>

 - Any tips for privilege escalation and information disclosure bugs?

   - ***Go to google and search "privilege escalation poc". Read all articles about it.***

<br>

 - Which skill do you have in programming?

   - ***Actually, I don't know any programming languages. If I need any information about it, I search it on google.***

<br>

 - How old were you when you found your first bug? What is your favourite bug type to hunt for?

   - ***3 years ago I found my first bug.***

   - ***Information disclosure (they are generally high severity).***

<br>

 - Which type of bug you look for? How much time you spend Hacking & learning every week? How much you made this year?

   - ***Classic bug types like xss, IDOR, info disclosure, business logical errors etc.***

   - ***I work 7-8 hours per day these days.***

<br>

 - How you balance bug hunting and learning?

   - ***I read disclosed reports and if I remember a similar feature on one of my targets, I try the same bug type in there.***

<br>

 - What's your strength when it comes to finding xss?

   - ***I put XSS payload to all inputs.***
