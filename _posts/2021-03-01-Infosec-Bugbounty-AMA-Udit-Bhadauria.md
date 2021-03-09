---
layout: post
title:  "Infosec Bugbounty AMA with Udit Bhadauria"
categories: infosec-bugbounty-ama
excerpt : "AMA with Udit Bhadauria"
author: Gurvinder Singh
---

# AMA with [Udit Bhadauria](https://twitter.com/udit_thakkur)

<br>

 - Q1. Which resources would you suggest(including guideline, tutorials, blog, courses, labs, toolset, methodology) for bug bounty?

 - Q2. How to combat with the negative sights of bug bounty? Like burnouts, duplicates, overcrowded researchers and resources, AI, massively tested programs.

   - ***For the first one, you can find the very detailed answer for this in my blog: <https://medium.com/hackcura/learning-path-for-bug-bounty-6173557662a7>.***

   - ***Bug-Bounty is more of a game. You win some, you lose some. So Duplicates is an indistinguishable part of it. The only thing is as long as you're okay with this, duplicates won't trouble you. And obviously getting duplicates is a clear symbol of, that you're on right path.***

   - ***To minimize the dupe, try to be more creative in your findings. And it comes with time and experience. Also that creativity idea can be come from write-ups, so make sure, you're reading blogs, disclosed reports regularly to ace your game.***

   - ***To avoid burnout, I personally think that a healthy routine &  proper sleep is must. Also anytime, if you feel like you're having burnouts, consider taking a break. And do what makes you happy like Traveling, Music etc.***

   - ***For the fact overcrowded researchers, You can't do much about it but to improve yourself and make an identity for you. And about the lots of resources, Cyber Security is vast. And no one can learn everything. There is redundancy. So pick something, learn it. Implement it.***

   - ***Proper note taking will help for sure. Learning is a life long journey. Don't think to learn everything, as it will overwhelmed you. About massively tested programs, everyone have got something unique. DoD/VMZ is the perfect example.*** 

   - ***Thousands of bugs have been reported still new bugs are being found. So give your best. Either you will find something or learn something. Its a win-win situation. And atm I don't think if any AI is smart enough to out smart human intelligence and creativity. Maybe in future. Who knows.***

<br>

 - How do you keep moving forward in hacking?

   - ***Constant learning and doing what I love and enjoy are the factors.***

<br>

 - Any weird bug you reported? Your most 3 favourite tools? Your most favourite public programs that you would love to hack on?

   - ***1. Weird bug.***

     - ***a. I was trying SSRF where it was converting the input data into PDF. Tried to read /etc/passwd for localhost. That eventually turned into DOS, where it wasn't getting anything for /etc/passwd and till the time PDF can not be generated next step not possible. Happened for Admin as the PDF was for feedback, that's copy will be sent to user.***

     - ***b. I was fuzzing the application for Stored XSS, where one payload accidentally broke the webapp that disabled the delete button for the admin, if end user will use the payload as name.***

   - ***2. Tools from [@pdiscoveryio](https://twitter.com/pdiscoveryio) especially Nuclei. (Made life easier) as custom templates friendly. Tools by the legendary [@TomNomNom](https://twitter.com/TomNomNom) and [@gwendallecoguic](https://twitter.com/gwendallecoguic) pentest tools.***
 
   - ***3. It was Dell earlier. Now a days I do mostly hunt on private. And want to dig into Indeed and VMZ surely.***

<br>

 - How do you approach a HTTP request smuggling bug? What are yur favorite bugs? What's your time management towards learning and hacking?

   1. ***Honestly I have never found Smuggling and XXE in blind but in Labs for me these two are the hardest ones. No comments.***

   2. ***Now a days its SSRF, PrivEsc and Business logic ones.***

   3. ***Most of the time its Hacking on weekdays and learning on weekends. So if I am acing my Automation, learning Python or studying for Certifications, I do it on weekends. But also, A little bit consumption of Youtube Infosec videos by [@codingo_](https://twitter.com/codingo_) [@InsiderPhD](https://twitter.com/InsiderPhD) etc, Newly published blogs, write-ups, [@Hacker0x01](https://twitter.com/Hacker0x01) Hacktivity on daily basis.***

   4. ***At very first, I found it really fascinating and now it is my primary source of income. I don't think if I need more reasons.***

<br>

 - How do you do Content discovery? I mean, finding new endpoints and parameters. Please include the info about the wordlists too.

   - ***Wordlist. I made a large one by merging number of famous ones like Raft, content_discovery_all.txt by Haddix and a few more. Tool I do use is ffuf. And for content discovery, I also do use gau and WaybackMachine by tomnomnom.***

   - ***For params and new end-point, I personally think that js files are gold mines. Also I do use hakrawler for crawling the site upto 3 level. And in burp I do use ParamMiner and for sites on CLI I go with Parameth.***

<br>

 - Q1. How to you select target?

 - Q2. How do you aproach a target?

 - Q3. What kind of bug you always look for and how can i find one?

   1. ***I usually go either with Wildcard scope or comparatively fresh single scope targets having access control (roles) and lots of functionality in them.***

   2. ***For big scope, I have few scripts that I made from various tools from github. Organized them in a way, that I used to do follow earlier. And regularly modifying it. Integrated it with slack for updating me. And then analysis of the result.***

   3. ***For single scope targets. At very first, I do start with low hangings (Mostly VRT P4) that can be found easily. And then I go through all the functionalities of web application by using it manually. Burp spider gives you end-point but using the web app manually gives better understanding of the application leads to better findings.***

   4. ***ATM I do focus mostly on SSRF and business logic. That can only be found by going through application functionality thoroughly. Keep trying, check all the functionality, try to build some unique idea how to abuse the functionality and you will find something definitely.***

 - Top github tool you use mostly while bughunting? What bug type you love to hunt on bugcrowd platform?

   1. ***[@pdnuclei](https://twitter.com/pdnuclei) by [@pdiscoveryio](https://twitter.com/pdiscoveryio)***

   2. ***SSRF, Business logic and if the program is fresh then at very first go for low hangings (Easy find).***

<br>

 - How do you choose targets to try out a specific vulnerability?

   - ***If target is having various roles like admin, guest, user etc. Look for IDOR, priv escalation. If site is kinda e-commerce. Look for race case, Price tempering, Blind XSS at address, feedback field, payment bypass etc. If site is having way to large scope, I do go for CVE Subd tko, information disclosure by directory fuzzing, github, wayback etc.***

<br>

 - How you manage your time with hacking and study, when you were beginner? What bugs you look for mostly?

   - ***In my beginner phase, I was in college. So it was like 9-4 college. 4-10 Dinner, fun, gaming and college work. 10-2 Hacking and Infosec Learning.***

   - ***Now a days, I do focus mostly on SSRF and business logic.***

<br>

 - What bug types you automate to find?

   - ***Pretty much automation can find majority of bugs. I have built many things working around using meg, nuclei, custom scripts, interlace etc. In my case, its subd tko, leaks on github, CVEs, directory listing, SSRF any many more. But always chances of dupe.***

<br>

 - Two advices for bug bounty with limitation in programming language?

   - ***Don't you dare to think that you can't be better in the game if you're not a hardcore programmer and coder.***

   - ***Don't think that you can only find bugs when you learn everything. Man just go and start trying with what you have. Learning is a lifelong journey.***

<br>

 - Five books and blogs you recommend?

   - ***Books:***

	   1. ***Real world bug hunting***

	   2. ***Mastering Modern Web Penetration Testing***

	   3. ***Web Application Hackers Handbook***

	   4. ***Owasp Guide (So much to learn there)***

	   5. ***Black hat python***

   - ***Blogs:***

	   1. ***[@intigriti](https://twitter.com/intigriti) Bug Bytes***

	   2. ***[@Hacker0x01](https://twitter.com/Hacker0x01) Hacktivity (Not a blog but disclosed reports are goldmine)***

	   3. ***Blogs published under [@InfoSecComm](https://twitter.com/InfoSecComm) on Medium.***

	   4. ***[@PentesterLab](https://twitter.com/PentesterLab) Articles worth reading last week.***

	   5. ***[@PortSwiggerRes](https://twitter.com/PortSwiggerRes) Archive.***

<br>

 - What is your recon process?

   - ***Its really a long one. Hard to describe in single tweet. But most of the things I have learned is from [@NahamSec](https://twitter.com/NahamSec) Twitch streams. And Bug Bounty Playbook by [@ghostlulz1337](https://twitter.com/ghostlulz1337).***
