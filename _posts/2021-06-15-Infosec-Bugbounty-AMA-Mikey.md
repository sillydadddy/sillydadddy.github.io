---
layout: post
title:  "Infosec Bugbounty AMA with Mikey"
categories: infosec-bugbounty-ama
excerpt : "AMA with Mikey"
author: Gurvinder Singh
---

# AMA with [Mikey](https://twitter.com/mikey96_bh)

<br>

## AppSec Engineer at Funding Circle, UK ⚙️ | Bug Bounty Hunter 🐞

<br>

 - Q1) How to choose my first program?

 - Q2) How long you take at a program to say it's secure and there is no bug .. let's move to another one?

 - Q3) What is your methodology from start to finish?

   1. ***Well that all depends on experience - personally I pick targets based on tech stacks that I like & the scope.***

	2. ***When I really buckle down on a target, I'd generally expect a finding or two within 1-2 weeks. If not sometimes and I like the app I stay but I tend to move on.***

	3. ***My methodology in a general sense is: 1) Subdomain enumeration (passive+brute-force), 2) Automated recon on these subdomains looking for functionality that I am interested in 3) Manually test the functionality as a user and capture the requests in burp-suite for manual inspection.***

<br>

 - What's your approach- Do you check for all vulnerabilities in one program or same vulnerabilities in different program?

   - ***I mix and match, if it is a web-application with a wide degree of functionality - I test all vulns on certain functionalities. If it is wide-scope, I look for one vuln across different subdomains, i.e. XSS.***

<br>

 - What are the Bugs which a beginner in bug hunting should concentrate more on?

   - ***Personally, I feel like XSS, CSRF & Simple Business Logic bugs are great learning points for beginners.***

<br>

 - Why are HTTP request smuggling writeups private? What can I do to learn better bug http request smuggling?

   - ***HTTP Request Smuggling can be hard to wrap the head around. <https://portswigger.net/web-security/request-smuggling> is the best resource I found for this - try out the lab too.***

<br>

 - What are your Favourite recon tools according to your methodology?

   - ***I use a combination of many, my friend [@dreyand_](https://twitter.com/dreyand_) has written a nice little tool call Andsu that does most of what I need. I tend to write my own tools to suit my needs for specific things. The tool is private for now anyway! I will post it if we ever release it.***

<br>

 - How to start my journey bugbounty?

   - ***Personally, I would not jump right in to bug bounty. Think of it like swimming you learn to swim before jumping in a poo. Take the time to learn the theory behind vulnerabilities and practice exploiting them - Pentesterlabs & Portswigger are great! You can use this to then try bug bounty.***

<br>

 - If you're a beginner and starting bug bounty, should you use pro version of the tools that you wanna use or is it okay to go with the community/free version and upgrade after your first bounty?

   - ***It is totally OK to use the free versions of tools and often ideal for beginners as you are forced to do everything manually and learn, rather than relying on active scans.***

<br>

 - As a beginner, how do I start in the bug bounty field? Is TryHackMe a good place to learn bug bounty or no?

   - ***Learn the basics first - I used the phrase don't jump into a pool when you can't swim earlier. It is the same here, do not jump into bounties without knowing the theory and practical stuff around a few bugs. It will make the experience a lot better.***

	- ***I really like PortSwigger and PentesterLabs that’s just my preference. You also have a lot of awesome creators who share free content!***

	- ***Personally I have only really used TryHackMe for OSCP prep. It may have more modules for Bounty related stuff but I can say the two I’ve listed previously were best for me.***

<br>

 - I've seen you mention a couple of times in blogs and tweets that you hack with a friend. Do you pick a partner who knows stuff you don't ? Or somebody who has a different methodology? Simply put, how to collaborate for the better?

   - ***I do like hacking with friends, especially those differently or higher skilled than I am. I think hacking with someone who does it differently to you is always great, you both learn along the way and come up with cool ideas together.***

<br>

 - How should one prepare for getting job profile of pentesting? How one should prepare for technical and interview round?

   - ***It all depends on what stage you are at, is it a first job? If so my best advice is have stuff to talk about at the interview - bug bounty was great for me. I know XYZ because I encountered it during this engagement is a great answer.***

<br>

 - Which wordlist you mostly use for subdomain brute force? What you think about assetnote best dns wordlist?

   - ***JHaddix all.txt, is what I started with I now use my own custom list.***

	- ***I have never actually used it, but I am going to go with that it must be pretty good if Assetnote have put it out there.***

<br>

 - What advice would you give for a beginner in bug bounties who is struggling to get bugs, facing a lot of burnouts and doubting his hunting skills?

   - ***Learn, learn, learn. I cannot stress this enough using the same tools, same methodologies will lead to the same outcomes. You have to look at your methodology and see where you can make changes for example learn better ways to do recon for a few months.***

<br>

 - After learning the web based vulnerability, on which platform a beginner should start to hunt?

   - ***I would pick a platform you like, personally I have to plug [@Bugcrowd](https://twitter.com/Bugcrowd) where I got started and have enjoyed every minute of it.***

<br>

 - Which is you favourite bug and which you hunt on most? At what age you started in Hacking field? Your advice for beginners? How much networking knowledge required, full networking concept or basic?

   - ***My favorite bug still has to be XSS, I started pretty late - I would say I maybe got my first bounty at 20. Enjoy yourself, learn and the money will come later. I consider myself to know the basics of networking.***

<br>

 - Can you suggest me any good checklist to do recon step by step?

   - ***I do not know about any published checklists but here is mines:***

	  - ***Enumerate subdomains & probe them.***

	  - ***Filter subdomains for interesting functionality - i.e via flyover or by looking at cookies.***

	  - ***Target those that fit criteria for what you like to hack.***

<br>

 - How did you actually got into this? I am reading some articles and doing portswigger lab but still it stucks on my head.

   - ***I started with programming, then one day I got fascinated with SQL injection when writing my own queries and it spiraled from there. My advice, take it slow, it takes years to learn it and you will never stop learning!***

<br>

 - How do you keep yourself updated?

   - ***Twitter is always a great resource for me for keeping up to date, I often see stuff here before I see it anywhere else.***

<br>

 - How to find interesting functionality of a program you hunt on? What subdomain name make you interested to hunt on is it : dev.\**.com or corp.**.com and so on?

   - ***Personally for me, I go with the larger scale recon and look at what is on the subdomain itself rather than just the name. Of course, dev, staging, corp & admin are always ones that catch the eye!***

<br>

 - I feel stuck without finding my first bug in Bugcrowd or Hackeone, how was your first bug found in bugcrowd?

   - ***My first bug on bugcrowd was actually in reference to one of my write-ups. I took a different approach that not many people were looking at and that’s how I got started! It was an info leak of 64M entries of PII.***

<br>

 - What are the tricks to bypass 403 error?

   - ***Just some of the top of my head, try to manipulate headers/the URL path to find ways around it. There are many write ups on this that are specific to certain tech stacks.***

<br>

 - How to expand target scope?

   - ***You should try subdomain brute-forcing you will be surprised by the results! Try out pureDNS.***

<br>

 - Is web development skills really necessary for bug hunting and what is one thing that benfits you while doing bug hunting like some previous achievements or the skills that you've learned in the past?

   - ***Web development experience is certainly not necessary but it helps. Most of the bounty platforms are blackbox anyway, however if you understand how certain features are "coded" then you have a better chance of thinking of ways to break them. Learning to read/write code certainly helps!***

<br>

 - Which certification is good for beginners?

   - ***I would go with eJPT, I have heard that is good!***

<br>

#### The original twitter AMA can be found here :- <https://twitter.com/sillydadddy/status/1404758530150658052>
