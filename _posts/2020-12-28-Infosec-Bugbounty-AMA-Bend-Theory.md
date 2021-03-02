---
layout: post
title:  "Infosec Bugbounty AMA with Bend Theory"
categories: infosec-bugbounty-ama
excerpt : "AMA with Bend Theory"
author: Gurvinder Singh
---

# AMA with [Bend Theory](https://twitter.com/bendtheory)

<br>

 - What should I do if the vulnerability does not come out after several hours of hunting when looking for a vulnerability?

   - ***I focus more on main web app testing and recon so I’m not as well versed as other hackers who go super broad with their recon. I currently use asset finder, subfinder, sublist3r, and google/github dorking to find subdomains.***

<br>

 - When you first started the bug bounty?

   - ***I became a Synack program manager at the start of 2018 which kicked off my initial interest in doing bug bounty myself. I was able to read and replicate hundreds of reports  before I even started hunting outside of work which was a great head start.***
 
   - ***I got my first bug triaged on a private VDP in summer of 2019 but I started hunting intensely after AT&T announced their public program on [@Hackerone](https://www.hackerone.com/).***

<br>

 - What are some evergreen bugs tips?

   - ***I found a fresh target and a vuln the other day by dorking for my target and using google’s feature to only show recently cached results and found a new subdomain and an easy XSS just a few minutes after that.*** 
 
   - ***Also, look for hidden input fields! the name/id attributes. It can sometimes reflect the values of query/body parameter names.***

<br>

 - Which resources did you follow to learn? And which practices and strategy made you a successful bug bounty hunter?

   - ***[Portswigger Web Sec Academy](https://portswigger.net/web-security) is a great resource for all bug types. I’m a bug bounty program manager first and a hunter second. My time as a manager reading reports helped me learn where/how/why web apps are vulnerable so reading lots and lots of reports and write ups.***
 
   - ***Also [@zseano](https://twitter.com/zseano) was a huge inspiration! I analyze javascript, google dork, and do deep main web app testing now because of him. go watch some of his youtube vids and check out his new project called [@BugBountyHunt3r](https://www.bugbountyhunter.com/).***

<br>

 - Any tips for beginners in this field?

   - ***Have a solid understanding of the following:***

      - ***HTTP***
 	  - ***HTML***
 	  - ***Javascript***
 	  - ***Basic web development***
 	  - ***Linux/Unix***
 	  - ***A scripting language of your choice***

   - ***If you don’t understand the fundamentals of what you’re trying to attack, you won’t find bugs. Also, don’t report clickjacking.***
