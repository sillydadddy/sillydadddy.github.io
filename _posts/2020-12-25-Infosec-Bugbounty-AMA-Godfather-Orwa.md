---
layout: post
title:  "Infosec Bugbounty AMA with Godfather Orwa"
categories: infosec-bugbounty-ama
excerpt : "AMA with Godfather Orwa"
author: Gurvinder Singh
---

# AMA with [Godfather Orwa](https://twitter.com/GodfatherOrwa)

<br>

 - Which tools that you mostly use and what is your recon map?

   - ***Tools***
     
 	 - ***[Dirsearch](https://github.com/maurosoria/dirsearch)***

 	 - ***[Amass](https://github.com/OWASP/Amass)***

 	 - ***[Nuclei](https://github.com/projectdiscovery/nuclei)***

   - ***Recon Map***

     - ***Shodan***

 	 - ***Github***

 	 - ***Google***

<br>

 - Say you just heard about bug bounties, what would the roadmap to your first bountyful bug be?

   - ***If i just heard about bounty, I will go and follow the new hunters and the old ones not the big hunters to start and know that's how this roadmap will came after that i will start learning the hard bugs not easy and down to easy bugs.***

<br>

 - How Do You Approach For Authentication Related Bugs?

   - ***I will use dirsearch and try to find end points from github.***

<br>

 - Which vulnerabilities I must look in very small scope target? ( E.g 1-2 subdomains only)
   
   - ***Think out of the box and search for all the scopes 'www.orwa.com', in scope 'blog.orwa.com', out of scope now they dont say '*.orwa.com' out so you can play here.***

<br>

 - What is the most interesting behaviour/bug you've found till now?

   - ***(Full Access For Admin Panel) with default credentials:

   admin panel page
   ask for user and password
   user:admin 
   password: password***

<br>

 - List five favourite dorks to find github information disclosure?

   - ***password***
   - ***pass***
   - ***secret***
   - ***pwd***
   - ***ldap***

<br>

 - How much time did you invested per day during your early days in this field?

   - ***In my first days, I started about 30 N/A for first month after that I start get duplicates and after that I started getting bounty.***

<br>

 - How do you pick your target?

   - ***I pick target that have small scope with bounty or points but small scope because lot dont test the small scopes.***

<br>

 - Do you do Manual Testing?

   - ***Yes, I do Manual Testing.***

<br>

 - How do you stay motivated?

   - ***I read about the new hunters tweet when they got first bounty.***

<br>

 - Do you do Automatic github dorking using any tool?

   - ***I do sometime. Check here [@obheda12](https://twitter.com/obheda12).***

<br>

 - What's your approach to sensitive information disclosure (apart from GitHub)?

   - ***Search in links and end points by github and google dorks.***

<br>

 - What type of file do you look for? The extension? And keywords for Google dork?

   - ***I look for sql extension and look for pdf files for the keywords which I shared on my twitter.***

<br>

 - What are your top 5 favorite bugs that you focus on? How much time do you spend bug hunting? Are you a full time bug hunter? When did you get you 1st bounty?

   - ***There are only (2): find secrets see what hide and Authentication Bypass.***
   
   - ***I spend 3 days in week coz i have another 2 jobs no not full time.*** 

   - ***I got my first bounty after i started learning in 6 days and that was 300$ form At&t [@Hackerone](https://www.hackerone.com/).***

<br>

 - If scope is small and no results in github dorks, you still you keep trying for information disclosure if yes what else you try? Or you try hunting other issues?
   
   - ***If I don’t find anything in GitHub,, I will go to google dorking and if that is not helpin, I will make these small scope a big scope for me. I will git all the sub sub domains and start test them but only report for the critical bugs P3 or P4.***

<br>

 - How do we ascertain the credentials like password API token key that we get are valid and how do we deal these credentials if it belongs to internal hosts of company?

   - ***That’s need a big big answer but the international rule is that if you find anything **Login out of scope** so simply report by that without login.***

<br>

 - In your amazing writeup you mentioned all your tips and tricks clearly but still do you have any other secrets with you?

   - ***No, I still have 1 secret that I forget to add. Check all the time your target on [Github Gist](https://gist.github.com/).***

<br>

 - How do you check your target what type of technology and programming language is being used on it??

   - ***I get all the sub domains by nuclei from nuclei and I check the bugs and technology.***

<br>

 - What learning resources have you followed in your journey of Bug Bounty? Were you involved anyhow in IT before Bug Bounty? How should we do bug bounty in 2021?

   - ***I dont have any background in it. I start to learn from the google and youtube and I learn only 2 courses for web pentest.***

<br>

 - What kind of bug should I choose to look for as my first bug?

   - ***Idor, Xss, learn for burp after that anything easy but in first you have to be good in 4 language javascript - php - html - sql.***
