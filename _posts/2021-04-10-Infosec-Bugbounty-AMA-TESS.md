---
layout: post
title:  "Infosec Bugbounty AMA with TESS"
categories: infosec-bugbounty-ama
excerpt : "AMA with TESS"
author: Gurvinder Singh
---

# AMA with [TESS](https://twitter.com/ArmanSameer95)

<br>

 - What’s your top 3 favourite bug bounty programs? Is it necessary to have burp suite professional edition for the beginner like me who’s just starting doing bug bounties?

   - ***To be honest with you, I don’t have any favorite programs and Burp Suite Professional is not necessarily important in the begining. I had Burp Community for almost most a year and I would advice you to stick with Burp Community and Better get a good understanding of it then switch to Burp Suite Professional.***

<br>

 - How do you approach already hunted target like who has around 500 bugs already reported?

   - ***If it’s wildscope, I would do asset enumeration, try to gather as much as subdomains possible, fingerprint they’re framework, bruteforcing directories, paths with [@assetnote](https://twitter.com/assetnote) wordlists depending on that cms but if you do asset enumeration and understand the Web-Application nicely.***

   - ***You will end up understanding alot of things and then go for they’re features such as anything lets say for e.g:- web application allows you to send emails as referral, I would say look for they’re employees emails and try to fuzz email parameters and play with the functionality.***

<br>

 - Tell me more about your subdomains gathering methodologies.

   - ***Aah! For subdomain gathering I use everything mostly <https://subdomainfinder.c99.nl> & <https://venkon.us/subdomain-lister/> and subfinder will all API keys , Findomain and assetfinder and most important Github & Pastebin too and then I sort all em out and screenshots with aquatoine and look for bugs.***

   - ***Best tool by [@0xMstar](https://twitter.com/0xMstar): <https://github.com/shmilylty/OneForAll>.***

<br>

 - What is your hunting methodology? Which is your niche bug (which type of bug you hunt most and focus on)? Any notes you can share?

   - ***My hunting methodology is mostly manually looking for bugs, If I started hunting on a target, I mostly learn what type of functionality they got and in what way I can abuse it, and focus mostly on cms based hunting like lets say IIS application then I would mostly run IIS Wordlist and focus on such bugs via reading other bug hunters reports on IIS based vulnerability.***

<br>

 - How do you keep yourself updated?

   - ***There's nothing specifically I do to update myself, but yes I keep reading reports on Pentesterland <https://pentester.land/list-of-bug-bounty-writeups.html> and mostly try new things or study new CMS/Framework.***

<br>

 - Do you have automation scripts? What is your approach on that stuff?

   - ***Mostly I hunt manually, I lack in automation but I’m trying to fix that. I'm trying to JavaScript so I can play with Vulnerabilities while exploiting them.***

<br>

 - What do you prefer more, hunting solo or hunting in squad and why?

   - ***Hunting with [@debangshu_kundu](https://twitter.com/debangshu_kundu) his research helps me alot.***

   - ***Mostly hunting with [@elmyuyu](https://twitter.com/elmyuyu) too.***
