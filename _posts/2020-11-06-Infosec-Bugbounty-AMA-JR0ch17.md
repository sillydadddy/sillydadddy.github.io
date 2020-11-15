---
layout: post
title:  "Infosec Bugbounty  AMA with JR0ch17"
categories: infosec-bugbounty-ama
excerpt: " AMA with JR0ch17 "
author: Ravi Shankar Gurram
---

# AMA  with [JR0ch17](https://twitter.com/JR0ch17)

<br>

## Bug bounty hunter, currently ranked 50th all-time on [@Bugcrowd](https://twitter.com/Bugcrowd).

<br>

 - how do you pick a target ?

   - ***It depends but I like scopes that don’t have many subdomains and have web apps with a lot of functionality. And of course, I look at programs’ bounty table, time to triage, time to bounty, etc.***

   - ***I also tend to look at programs that have top hackers in the leaderboard. I find it fun and challenging to look at a program that has been looked at by others, it’s nice when I find bugs that they missed or didn’t think of!***

<br>

 - What keeps you motivated?

   - ***I think what keeps me motivated is that I want to be a better hacker than I was yesterday. I love learning and I try to learn as much as I can every single day!***

<br>

 - How you deal with burnouts?

   - ***I don’t really deal with burn outs since I don’t let myself get to that point. I manage my time in front of the screen correctly. I hack once in a while on week nights and practically never on weekends.***

<br>

 - Any idea how to change the mentality of this "app is already tested by a lot of pros"?

   - ***We all think differently, we don’t have the same thought process so don’t assume that another hacker looked at a specific feature and it’s secure. Maybe the way you see it and is totally different than others and maybe you’ll think of something that others didn’t try!***

<br>

 - If you could go back in past and talk to younger-self who is starting bug bounties, what will be your suggestions/tip/tricks to him.

   - ***I’d tell myself, don’t quit school and learn how to code lol I never finished my degree and I realized recently that I love to code even if I’m not an expert doing it. Approaching my 30s and with a family and bills to pay, I can’t easily go back to school and finish up my degree***

<br>

  - Is it worth to learn bug bounty hunting nowadays? If not then should I focus on learning appsec, code auditing, penetration testing or red teaming to get a job?

    - ***It’s never to late to learn bug bounty! I can’t really answer, it’s really up to you and what you love doing and what you’re passionate about!***

<br>

 - What basics you done before starting and doing bugbounty and how much time you spend on basics.?

    - ***I worked as a sysadmin for like 5 years before I started hacking so I had basics in networking, Linux, etc. I had also done the OSCP certification before I started doing bug bounty so I knew the basic stuff already. Then I dived into web app stuff for like a year or so.***

<br>

 - Focusing  on one bug is better or more while  learning.?

    - ***While learning, I think it’s good to focus on all bug types. That way, when you start doing bug bounty, you’ll feel comfortable and confident to find all sorts of bugs, and not just the regular stuff like XSS and IDORs.***

<br>

 - What Burp extensions  you use..?

    - ***I use plenty of extensions but I only enable some of them depending on what I see on the application. I usually have these enabled all the time: Logger++, Hackvertor, Param Miner, Content Type Convertor.***

<br>

 - What you recommend  manual or automation.?

   - ***Automate as much as you can, that way you’ll have more time to hack on other stuff. I’m not really a subdomain recon guy, so I normally dive right into web apps with Burp so I don’t have much automation going on a part from the tool I built.***

   - ***only the subdomain enumeration part of my recon is automated. As for the rest, I prefer the manual approach at hacking web apps. I don’t even use Burp Scanner, I’m a heavy Repeater user and use Intruder once in a while to fuzz!***

<br>

 - What does it takes to be where you are at now.

   - ***Hard work, dedication and perseverance!***

<br>

 - Programing languages to learn for bug bounty?

   - ***Not required but I recommended learning at least one programming language like Python, Go or Ruby. I also recommend learning JavaScript if you’re interested in web apps. JS is every where now so  it’s good to know.***

<br>

 - Do you recommend For beginners To do CTF or pentesterlab ?

   - ***I’d say Pentesterlabs since I find it’s more realistic than CTFs. Not saying CTFs are bad it’s just that sometimes depending on the CTF, you’ll do stuff that you’ll never do in bug bounty or pentest. I’d also put in [@WebSecAcademy](https://twitter.com/WebSecAcademy) in there as well, awesome resource to practice!***

<br>

 - Any podcasts you follow to get latest cyber security news

   - ***I don’t really listen to podcasts. I take a look at Twitter every day to see if anything new has come up. As for the rest, I’m subscribed to [@intigriti‘s](https://twitter.com/intigriti) bug bytes. It’s a great way to look at anything that has come up in the past week that I might’ve missed.***

<br>

 -  what is your recon methodology? what automation you use for recon

    - ***I do subdomain recon first and everything that comes with it, so screenshots, I grab response headers and body, port scans, I grab what technologies are used, DNS info and store all of that in my database. I built (still in progress) a web app tool that does all of this for me.***

<br>

 - what u look first(bugs) for when u get a target or a API endpoint.

   - ***The bugs I look for first depends on what type of API I’m looking at, what the endpoint is supposed to do, what technologies are used, etc. There’s not really a bug type I look at first, though I always look for server-side bugs first.***

<br>

 - you do js enumeration or not if yes then what is the process and tools you use.

   - ***I don’t really have any js automation in place, I prefer looking at it manually in VS Code. I do sometimes use tools like LinkFinder to find endpoints but most of the time I go through the code manually in VS Code or in Chrome’s Dev Tools.***

<br>

 - Do you use any automation for github recon?

   - ***I used to automate GitHub recon but I stopped since I never really got anything good with it, I think I only got 1 bounty because of it. Now I typically just look for specific stuff manually.***

<br>

 - How can i automate for SQLi like what are the responses and patterns ?

   - ***When looking for SQLi, it’s important to check if there are any error messages that indicate whether it’s potentially vulnerable or not. Sometimes it’s blind so you want see anything. That’s when we need to use time-based payloads.***

   - ***It’s not always easy to detect and find, when I feel like it’s vulnerable but can’t get anything to work, that’s when I use sqlmap.***

<br>

 - What Linux tools do you use to find vulnerabilities? Also, when injecting an attack vector to find sqlinjection, what attack vector is injected and diagnosed?
Example) q=1, pw=8&t=te
q=' and sleep() -, pw=8&t=8-sleep()

   - ***I use tools like fluff, sqlmap, ysoserial and others for specific stuff or exploits. I’m not sure I fully understand your SQL injections, but I simply try the basic stuff first without even putting payloads right away. Putting in sleep() is useless if Postgresql is used!***

   - ***I don’t really use the spray and pray approach, I try and go logically to avoid wasting time sending in requests that simply won’t help me. I try to think what kind of SQL query it is, what DBMS, etc to do a more targeted attack.***

<br>

 - In your beginning days before finding your first bug how many hours you used to hunt in a day?

   - ***When I started hacking, I used to spend 10-20 hours per week.***

<br>

 - Finding a right target is very difficult for a beginner as many of them are already hunted by some good hackers. which type of targets you used to select in your initial days.

   - ***I actually started looking at VDPs when I started. I think it’s a good place to start, get some experience, find bugs and with all of that you’ll receive private invites!***

<br>

 - What bug type u find the most ..and what bug u lov ...?

    - ***I’d have to look at my stats but I think what I find the most is either XSS (any sort), SQLi or Path Traversals.***

    - ***I love anything server-side, so RCE, SSRF, SQLi, Path Traversals, etc. It’s typically what I spend the most time trying to find.***

<br>

 - How do you approach single scope programs, what bugs will you search for and what would your methodology be like on that program?

    - ***Normally I browse around the application like a normal user would, just to get a feel of how the application works. And in the mean time I look at what frameworks and technologies are used on the application and I’d start fuzzing around and try to find bugs!***

    - ***I don’t look for specific bug types, I test for different bug types depending on what the request does!***

<br>

 - How do u take notes while looking the through the web app.

    - ***I’m pretty bad at taking notes actually. If I have to take note of something I put it directly in the comment column in Burp Proxy History. Some times I put notes in a txt file as well.***

   - ***I also log every in-scope request to ElasticSearch so that I have a history of it. So if I need to look something up, I simply need to query ElasticSearch. A lot easier than going through each Burp project!***

<br>

 - How many requests you view in Burp a day? Do you read all of them or only the ones you are interested in?

   - ***Not sure about the amount on days that I hack but it’s for sure a lot*** 😛 ***I typically have certain filters in place that removes the one I don’t care about.***

<br>

 - As a power user, what are your favorite burp tricks?

   - ***One thing I can say though, is that I love shortcuts, I don’t think I use a mouse when I use Burp.***

   - ***I feel like most of the stuff I do with Burp is all well known now. That said, I rely on Grep Match and Grep Extract a lot when using Intruder, I do a lot of stuff with Match and Replace as well in the Proxy Options. I just try and make sure I use Burp to its fullest*** 😛

<br>

 - How have you applied your javascript knowledge and translate that into award-winning vulns? :P

   - ***Award-winning vulns*** 😂 ***Honestly it’s just with practice and actually building my web app in Node.js. I also learned a lot from [@TomNomNom](https://twitter.com/TomNomNom), [@filedescriptor](https://twitter.com/filedescriptor) & [@Corb3nik](https://twitter.com/Corb3nik) so shout out to them*** 👌

<br>

 - How to you proceed after finding Subdomains or URLs using gau or waybackurl ?

   - ***I take the list of URLs and put them in a file. Then I have a small bash script that runs curl for every URL in the file. I also have the proxy option in curl so that I can see the results in Burp Proxy History.***

<br>

 - Suppose you got lots of subdomains and some open ports on them Then which port you usually look for to start with? What are the good ports to looking for pentester wise ?

   - ***I look at other common web ports like 3000, 7001, 8443, 4443, 8080, 9001, etc. Often times these ports run some sort of admin panel.***

<br>

 - How do you approach a bunch of subdomains for hunting

   - ***I built a tool that does all of my subdomain recon. I take screenshots, I grab response headers and body, technologies used, DNS data etc. I then pick web apps that have technologies that I’m familiar with or I look at the screenshots to find subdomains that look vulnerable.***

   - ***But since I prefer the manual approach, I typically look at the core app first (ie. http://domain.com) and then look at other subdomains after.***

<br>

- in a high level how is your approach when you fuzz? First you try to obtain verbose errors? If so, you go crazy with your wordlists? i.e special chars, null bytes, nasty strings, diff unicode encodings (UTF-8/16/32), HTML entities (d, hex)?

  - ***Yeah so first I try the basic stuff in Repeater. If that doesn’t work then I do pretty much what you mentionned, I send it as much as I can and look at how the application reacts. It doesn’t always work, but sometimes it does!***

<br>

 - I wanna know your fuzzing process , like do you fuzz everthing from urls , cookies , body parameters , or you look for specific parts to fuzz , and how you approach a part that is vulnerable but there is no response indicating that is vulnerable

   - ***Most of the time it’s from URL and body params. But some times, depending on what I see, I fuzz cookies and certain headers, especially unique headers that are specific to the application. I’ve had cases where I had auth bypasses and LDAP injection when fuzzing those headers!***

   - ***When there’s no indication that it’s vulnerable, I try and think of what exactly it’s doing and what technologies it’s using in that particular request so that I can do more of a targeted attack.***

<br>

 - How do you bypass 403 forbidden page ,  techniques you can share that works in maximum cases !!!

   - ***It really depends on the use case, what technologies are used, what is causing the 403 forbidden, etc.***

<br>

 - Which is the most unknown Security flaw ? 🤔

   - ***Hmm well if it’s unknown than I don’t know it*** 😛 ***that is a bit uncommon but that is gaining in popularity these days is Prototype Pollution.***
