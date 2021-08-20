---
layout: post
title:  "Infosec Bugbounty AMA with payloadartist"
categories: infosec-bugbounty-ama
excerpt : "AMA with payloadartist"
author: Gurvinder Singh
---

# AMA with [payloadartist](https://twitter.com/payloadartist)

<br>

## Hacker 🐱💻  Part of [@SynackRedTeam](https://www.synack.com/red-team/) & [@Detectify](https://detectify.com/) 🔥

<br>

 - Q1) How to be a part of synack red team?

 - Q2) In your perspective, what bugs to look for consistent earning?

 - Q3) How to be well versed in crafting our payloads?

   1. ***Apply with your resume if you feel you are a good fit. My friends [@impratikdabhi](https://twitter.com/impratikdabhi) and [@ozgur_bbh](https://twitter.com/ozgur_bbh) can potentially help you with a referral to fast track the application process.***

   2. ***Getting a good grasp over Owasp Top 10 should be enough.***

   3. ***Crafting payloads should be specific to the application you are testing, and the WAF and filters they are using. For example seeing how an input is getting reflected and how the backend is processing it could help crafting the right payload. It needs a lot of experience.***

<br>

 - Which parameters do you look for while hunting?

   - ***‘Url’, ‘to’, ‘next’, etc are interesting for me as they often end up in open redirect or SSRF. [@0xAsm0d3us](https://twitter.com/0xAsm0d3us)’s tool is quite useful for finding interesting/hidden URL parameters: <https://github.com/devanshbatham/ParamSpider>.***

<br>

 - What learning resources do/did you follow in bug bounty? Which tools do you use? Do you approach for certain sets of bug or hunt for as much as possible?

   - ***Mostly by reading Write-ups by others. Subfinder, Knockpy, waybackurls, gau, Nuclei, GoWitness, Gobuster there are a lot of them and my own scripts. All types of vulnerabilities.***

<br>

 - Can you suggest some good resources to learn Pentesting topics and which certification is best: eWPT or eCPPT?

   - ***For pentesting [@hackthebox_eu](https://twitter.com/hackthebox_eu) and [@PentesterLab](https://twitter.com/PentesterLab) labs are pretty cool if you want to gain hands on experience.***

   - ***As for certification I can’t say, as I don’t have any but the most in demand are OSCP and CREST afaik. Not sure about the ones you mentioned.***

<br>

 - What's automation all about in BB? How can we do by ourselves? Any resources or Tips?

   - ***If something that’s otherwise done manually can be automated, it makes the process much more efficient than manually performing it.***

   - ***Examples can be, scanning targets, tracking changes in the client side JS code, & performing content discovery in a periodic manner.***

<br>

 - How did your journey start in Infosec? Who motivates or guide you?

   - ***Journey in Infosec began with getting curious about hacking and an urge to master the art of the hackers.***

   - ***[@zseano](https://twitter.com/zseano) is a big motivation, back in the day I found a vulnerability in Google after reading one of his old articles also he’s a great human.***

<br>

 - What are your favourite GitHub repositories and why?

   - ***You can have a look at the repos I have starred on Github - <https://github.com/payloadartist?tab=stars>, because I find them useful. I suggest going through [@m4ll0k](https://twitter.com/m4ll0k)'s and [@tomnomnom](https://twitter.com/TomNomNom)'s scripts in particular, very interesting stuff- <https://github.com/m4ll0k/Awesome-Hacking-Tools>, & <https://github.com/tomnomnom/hacks>.***

<br>

 - What are the common bug you get encounter in every other websites which is P1 or P2?

   - ***Mostly I like to find information disclosure through recon often a particular misconfiguration in a widely used software for example. Mostly varies between medium and high.***

<br>

 - Any cool burp extension which could help me in Bug Hunting?

   - ***Logger++ is a very handy Burp extension. It logs all requests from the testing you do, then you can grep for a particular thing like an SQL error in the response  with custom queries as you can see below.***

<br>

 - Any cool browser add-ons for Bug Hunting?

   - ***Tamper Dev by [@sirdarckcat](https://twitter.com/sirdarckcat) is a cool intercepting proxy, its got a nice UI and some neat features if you want an alternative to Burp: <https://chrome.google.com/webstore/detail/tamper-dev/mdemppnhjflbejfbnlddahjbpdbeejnn>.***

   - ***PostMessage-tracker by [@fransrosen](https://twitter.com/fransrosen) for finding postmessage vulnerabilities: <https://github.com/fransr/postMessage-tracker>.***

<br>

 - What do you think are some of the basic bugs for a beginner to start with?

   - ***As a beginner, can start with the [@WebSecAcademy](https://twitter.com/WebSecAcademy) they have the most well structured course in my honest opinion (not paid by them to say so). Just go through their course material, labs and decide for yourself what you are most interested in.***

<br>

 - I started with SQL injection (learned it frm portswigger's web sec academy) and I failed to find them. Which bugs should beginner focus to find first as starting?

   - ***Try to get a good grasp over all Owasp Top 10 bugs, you can also try Owasp Juice Shop and such vulnerable apps. Most applications nowadays are very hardened so spend some time analyzing the app and understanding where there maybe bugs.***

<br>

 - What are some recommended Bypassess for html encoding? White papers would be appreciated.

   - ***If the sanitisation is done by means of a weak regex you can try breaking the regex logic somehow. Consider going through Owasp XSS evasion cheat sheet. [@s0md3v](https://twitter.com/s0md3v) has written a good paper on XSS bypasses: <https://github.com/s0md3v/MyPapers/tree/master/Bypassing-XSS-detection-mechanisms>.***

<br>

 - If you count your all time you spend on learning how much it is, and if you do it using 100 percent then how much it would be?

   - ***I don’t think you should provision say a certain % or ratio of time into learning. Learn as much as you can without feeling overwhelmed and try to put it into practice at the same time to test yourself.***

<br>

 - Should I focus on learning one bug and be better at it, rather than study all bugs of portswigger? So later when I want to do bughunting I'm gonna search for one bug or two on the program?

   - ***It’s more like asking whether to focus on a single type of vulnerability to become a pen tester. When you are on an engagement you are supposed to be familiar with most if not all classes of vulns so you are able to test any app. Same applies to bugbounty.***

<br>

 - What’s your methodology on approaching old programs or wide scope programs? How do you spread your attack vector?

   - ***Usually reconnaissance (active + passive) to understand the target. Then narrowing down the testing to a particular application in scope that appears interesting.***

   - ***Often I look for certain software misconfigurations and a particular type of information disclosure.***

<br>

 - How does your approach towards a program look like? How much time at least you give to a program you start hunting upon?

   - ***Usually reconnaissance (passive + active) to begin with. I mostly hunt on applications I regularly use and familiar with. So effectively, spend a lot of time with the applications. The goal is to get well acquainted with the app’s features first.***

<br>

 - How to be better at writing our own exploits?

   - ***Afraid to say I am not competent enough to answer this as I am not an exploit author. But I think you can try solving CTFs that need you to write exploits or try picking up recently disclosed PoCs and try writing exploits yourself.***

<br>

 - Please share your unique or weird or awesome experience with your bug bounty findings.

   - ***Getting access to extremely sensitive data (including cc data) of few million users on multiple applications, then getting paid $500 for it on a private program on Hackerone.***

<br>

 - What you do when you are stuck at finding vulnerability?

   - ***Try harder? Yes and no. But if it’s beyond my capability I usually move on.***

<br>

#### The original twitter AMA can be found here :- <https://twitter.com/sillydadddy/status/1395956648158449665>
