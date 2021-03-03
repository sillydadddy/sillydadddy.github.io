---
layout: post
title:  "Infosec Bugbounty AMA with Nagli"
categories: infosec-bugbounty-ama
excerpt : "AMA with Nagli"
author: Gurvinder Singh
---

# AMA with [Nagli](https://twitter.com/naglinagli)

<br>

 - Some tips for beginners in this field?

   - ***Watching this talk by [@zseano](https://twitter.com/zseano) <https://youtu.be/-6tv1kvBZDQ> and going over H1 disclosed reports here <https://github.com/reddelexc/hackerone-reports> by bug-types. Write up some intersting vectors presented and try them on less populated BB programs.***

<br>

 - Tips and resources for IDOR and ATO?

   - ***You can check my blog with ATO due to IDOR on the DoD, honestly id look for old looking login pages and account portals to see if there is wrong implementation with numerical id's. Link: <https://galnagli.com/DoD_IDOR/>***

<br>

 - Tell us your story in bug bounties.

   - ***Started approximately at April by studying Stanford CS253 course, found few rate limiting bugs but nothing more, took a break to study from writeups and streams and started to get results around August, assembling my own recon automation rewarded me the most as by knowledge and $.***

<br>

 - Any weird bug that you reported to the company?

   - ***I was looking on some DoD websites with manual google dorking recon, one site caught my eyes with weird authentication, I tried navigating to redacted[.]com/admin and surprisingly got authenticated as administrator.***

<br>

 - How you approach your target, like you do recon deep or just start shooting its root domain or have any specific endpoint, technologies that you shot first?

   - ***Whenever i'm engaging with a new TLD I run my full recon script which consists (subfinder,github,shuffledns,assetfinder) -> running port scan on those with naabu -> nuclei them all -> gathering endpoints with waybackurls/gau and sorting by GF patterns + kxss.***

   - ***Meanwhile engaging with the main page, I try to inject \<h1>nagli\</h1> on every stored parameter (such as name) which could be rendered on marketing emails. Navigating to most of the functionalities which will get captured with burp and observing the burp bounty profiles.***

   - ***I am using a booklet of notes to try whenever faving a certain type of functionality, and in general what areas to look for when there isn't anything imminent, such as shodan and external services for leaks dorks. One thing I want to create in 2021 is a GUI DB based automation.***

   - ***As i'm hunting lately on public and private crowded BB programs I don't expect finding any RXSS or HTMLI by query param injections, so trying to achieving those by different vectors.***

<br>

 - How do you manage between bug hunting and school?

   - ***I study on "Open University", taking 2 courses each semester instead of 4 like on other universities allowes me to work full time and Bug Bounty occasionally.***

<br>

 - Q1: How to pique our interest in a topic? Q2: Whenever i decide to hack i get a sensation that i'm not ready to hack yet and i back down, how do i get over this? Q3: Any Life Hacks,Tips or Advice for the upcoming generation?

   1. ***Think about what you will gain when you master that specific topic.***

   2. ***Try hacking on wildcard scopes VDP, no stress ehen hacking and it will build confidence.***

   3. ***I'm still pretty new my self but you need to understand how the system works to break it successfully.***

<br>

 - How much time do you give for learning and hunting?

   - ***Learning whenever possible through reading writeups abd checking twitter feed, hunting mostly 2 hours at weekdays and on weekends.***

<br>

 - How do you pick target bro? Bugs you will be looking first? Most common bug you found in your testing?

   - ***Reflected XSS through Open Redirect is the bug I have encountered the most and on some big orgs (HackerOne/BugCrowd/AT&T etc..) I'd look for third party systems integrated under the TLD and test for bugs on those - it means that the target inherits their security issues.***

<br>

 - Do U Have Any Private tool Automating Your Recon Process? Do U Like Github Recon?, How do u look for those bugs? Do U Have Any tips for noobies Like me? How Do U Keep Motivated?

   - ***Yes, it's private just because I didn't bother to code it nicely, there are many open source tools which makes the same actions I'm doing, it's just better to understand the code you are using and to integrate it the best way so it would work for your needs.***

<br>

 - Which one do you think is better and why? Spending a lot of time on one program or just move on?

   - ***Probably sticking to top 5 and running automation of nuclei on all other targets, bigger chance for good vulnerabilities.***
