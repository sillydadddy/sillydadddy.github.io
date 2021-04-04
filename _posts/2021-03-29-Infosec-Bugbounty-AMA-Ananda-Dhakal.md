---
layout: post
title:  "Infosec Bugbounty AMA with Ananda Dhakal"
categories: infosec-bugbounty-ama
excerpt : "AMA with Ananda Dhakal"
author: Gurvinder Singh
---

# AMA with [Ananda Dhakal](https://twitter.com/dhakal_ananda)

<br>

 - How should one start with Hackerone? How did you started?

   - ***It's almost the same as Bugcrowd but HackerOne requires quite a practical impact for the bugs to be accepted. It wouldn't bother you since you find heck a lot of P1s. I have been hunting on Hackerone since I started bug bounty so I am more comfortable with it.***

<br>

 - Can you give some tips about OAuth bugs if you find some of them please?

   - ***Check this out for OAuth bugs: <https://medium.com/a-bugz-life/the-wondeful-world-of-oauth-bug-bounty-edition-af3073b354c1>.***

<br>

 - Tips for approaching a single scope/medium scope target?

   - ***At first, you should understand the features and the functionalities that the application has. Play around a little bit to get familiar with the application.***

   - ***Test every functionality by asking yourself, "How can I abuse this behavior?" That's how you get most of the bugs.***

<br>

 - How do you approach of SSRF? Which tools you used for SSRF?

   - ***I am not quite an SSRF hunter but wherever I see any functionalities that deal with URLs, I try my way for SSRF.***

   - ***I don't use any tools for SSRF.***

<br>

 - What is your hunting methodology? Which is your niche bug (which type of bug you hunt most and focus on)? Any notes you can share?

   - ***I don't have a specific methodology like others but I mostly focus on the main application for the vulnerabilities.***

   - ***I really love to break the logic of the application and get the bugs!***

   - ***Well, I don't take notes.***

<br>

 - Would you recommend any bugs to focus on, it's been more than few months, I haven't got any single bug?

   - ***Learn all the bugs, focus on the bug that catches your interest, and dig deeper into that bug. Have patience and most importantly, don't give up.***

<br>

 - What is the most common mistake you make while hunting and what are the resources you used to learn hacking and last what how long to your prefer to test a single parameter or target?

   - ***No mistakes as far as I know.***

   - ***All blogs, writeups, and videos related to hacking and bug bounties really helped me at the beginning.***

   - ***If the target is interesting, I like to test for longer. If the target doesn't catch my interest, I leave the program after some days.***

<br>

 - How do you approach a target? What are the methodology you used for small scope? If there is no sign up/login page... What bugs I should concentrate at?

   - ***Mostly, I start the direct test after scanning all the subdomains. If I find anything interesting, I start digging into it.***

   - ***For the small scoped program, I try to understand its features and logic. Then, I test for some common bugs like CSRF, IDOR and access control bugs and authentication-related issues. After that, I focus on business logic vulns mostly and try to exploit the features with broken logic.***

   - ***I look out for directories that leak sensitive information and sometimes XSS on hidden params as well. Mostly, I skip that type of site.***

<br>

 - Your top 3 bug classes? How do you manage between hacking and learning?

   - ***Access control and authorization issues.***

   - ***Business Logic Issues.***

   - ***Request Tampering.***

   - ***Hacking and learning need to go hand in hand. If you stop doing one, the other has no value.***

<br>

 - How you hunt for information disclosure bug? Please share your methodology.

   - ***For information disclosure: Google Dorking, Github repo, directories leaking sensitive info, playing around with requests, and many more.***

   - ***I do not have a specific methodology but usually, I target the main application and start hunting on it.***

<br>

 - What is your daily schedule looks like, and how many hours you do hacking everyday?

   - ***I am not hacking much lately due to high-school. It takes my time from 7 AM to 3 PM.***

   - ***After that, I do remote work, surf the internet, a little bit of guitar, and a little bit of studying, and the whole day is just finished. After having dinner, I do some hacking stuff and sleep.***

<br>

 - How do you approach a target when you are looking for sub domain takeover and which specific tools you use for it? Also share your thoughts about sub domain takeover vulnerability in general.

   - ***All my subdomain takeover testing is automated. I use SubOver for subdomain takeover but I have made a lot of changes on tool to make it more useful.***

   - ***There is a lot of competition for the subdomain takeovers. Manual testing for the issue is not really worth of time. Automate it.***

<br>

 - What if I take out all subdomain using different tools like sub-finder, sublister, Amass and then look for subdomain take over if any?

   - ***That's good to go but try to automate the subdomain takeover testing as well.***

<br>

 - Q1) What bug you look for in starting and now .... also how to master those?

 - Q2) Also what you do in free time and to fresh mood?

   - ***The bugs I looked at and still look at are mostly logical issues (putting aside the technical bugs that I hunt for as well). To master it, you need to develop the thinking of a hacker and thinking out-of-the-box.***

   - ***Guitar, anime, a ride with [@dhakal__bibek](https://twitter.com/dhakal__bibek) and many more things...***

<br>

 - Any weird bug you reported which you are proud of?

   - ***It's not really something that I am proud of but there was an application that reset the password when signing up using the same email again. It was considered low since the issue was in the staging environment.***

<br>

 - Do you look for SQLI, XXE?

   - ***I don't usually. Yeah, right but still nothing is hackproof.***

<br>

 - Which kind of bug should i search for as my first bug?

   - ***You can start with any bug you want. Learn the basics of all bugs and start with the one which you find the most interesting.***

<br>

 - Is there any specific business logic bug, you focus the most when testing some ecommerce website?

   - ***No, there is no specific bug I focus but you can test for price manipulation issues mostly on e-commerce sites.***

<br>

 - How to show impact of open redirection by referer header?

   - ***Not practically exploitable unless you chain it with cache poisoning.***

<br>

 - Tips for a would-be graduating student on breaking into the Security industry, i.e getting the first job or internship?

   - ***Just keep learning and keep doing. Give the best you can.***

<br>

 - How do you deal with a burnout?

   - ***Anime, travelling and hanging out with friends. I do not force myself too much so that I can avoid burnout, prevention is better than cure.***

<br>

 - Are you still getting same amount of bugs like before? Or getting less than that due to the unhealthy competition and craze of different types of security researcher?

   - ***The amount of bugs I am finding nowadays is almost the same as before but to some extent, it's harder than before. Be unique in your findings and it will not be a problem.***

<br>

 - If you have a big scope, how do you do port-scanning?

   - ***I don't do it.***

<br>

 - Any specific bug to hunt on the new target?

   - ***Hunt for every bug that you possibly can think of.***
