---
layout: post
title:  "Infosec Bugbounty AMA with Shashank"
categories: infosec-bugbounty-ama
excerpt : "AMA with Shashank"
author: Gurvinder Singh
---

# AMA with [Shashank](https://twitter.com/cyberboyIndia)

<br>

## 🛡️ Ex-Security Analyst at HackerOne 🛡️ | 🔑 Team Lead at [Cobalt.io](https://cobalt.io/) 🔑 | 🐞 Part-time Bugbounty Hunter 🐞

<br>

 - Any soft skill suggestions for me? How can I learn research skills and build up an organized methodology?

   - ***Soft skills: I think that is more of a self-personality with good communication skills. This is mostly developed in schools and colleges or with people around you, and obviously, your work environment teaches you a lot.***

   - ***Research is a continuous process. I would suggest reading daily. Read all disclosures and I think Twitter is the best place for that. Don't just scroll read all the writeups and save them for future reference if required.***

   - ***Another good habit is to google. When you are looking for bugs. If you don't understand anything google it out. Never ignore anything you didn't understand. Once all knowledge gets accumulated you will be able to organize it in your own ways.***

<br>

 - What is your hunting methodology? Recon process? Which is your niche bug (which type of bug you hunt most and focus on)? Any notes you can share?

   - ***Recon:***

   - ***I have my own setup. I have dockersied amass, subfinder which passes subdomains to ffuf and waplizer. It also finds all the IP and runs main templates of [@pdiscoveryio](https://twitter.com/pdiscoveryio) nuclei. After the scan is complete it sends it to my slack.***

   - ***It is a continuous process. I have been doing it for years. Writing the base took few weeks.***

   - ***Niche Bug:***

   - ***I love access control bugs. I prefer to read the docs and APIs and find IDOR or privilege escalations. I feel these are always overlooked because most hunters don't read the API docs and focus way too much on recon. I have fewer dupes here.***

   - ***The tool is quite scalable as I can adjust the number of parallel containers I can spawn. And I can choose which tool to skip and adjust according to the program and my server resources. I will suggest writing your own scripts.***

<br>

 - Q1) Which learning materials did/do you use?

 - Q2) Which tools do you use?

 - Q3) Which vulnerabilities do you look for when you approach a target?

 - Q4) How do you pick a program?

   1. ***My best learning platform to this date is twitter. I follow everyone who tweets writeups and I keep my feeds clean. I do daily reading. Another way is I just go to a hall of fame page and visit the hunter's blog.***

   2. ***I use everything which I find handy. The most common ones are amass, subfinder, ffuf, Burp suite pro, project discovery tools. I do write my own stuff as well: <https://github.com/Shashank-In?tab=repositories>.***

   3. ***I am a fan of access control-related issues. I love testing APIs. I feel they are overlooked, and people focus way too much on recon rather than learning the application and finding bugs in it.***

   4. ***I mostly hunt on a program that I actually use or want to learn about the application. Also, I work a lot on public programs. It helps me to build a relationship with the companies as well.***

<br>

 - Q1) What is your approach for XSS vulnerability (automation + Manual approach using tools)?

 - Q2) Some of the tools which you use for recon process?

 - Q3) Any learning resources for bug bounty hunter?

 - Q4) If a domain http://abc.com is given to you for hunting what is your approach?

 - Q5) How do you approach each functionality of the website (eg: login page,invitation etc) like each functionality what and all bugs can be found?

 - Q6) How do you find latest CVE effecting the given http://abc.com website?

 - Q7) Mention any forums where we can stay updated with CVE and new bugs.

   1. ***Manually test whatever is infornt of you and meanwhile let burp crawl all the endpoints. Then I use the burp scanner's module which tells you about reflections. So it will flag all the input which is getting reflected inside the body.  Now send all the reflections to the repeater and look for an XSS manually. Remember burp's XSS scanner is not finding all bypasses. For stored XSS. You need to have an eagle's eye. To remember what is getting reflected where.***

   2. ***My recon process. I discussed it here: <https://twitter.com/Djin54502490/status/1387436632832311302>. Also I am fan of Haddix: <https://hacker101.com/conferences/hacktivitycon/tbhm.html>.***

   3. ***I have compiled few of the learning resources here. Since twitter allows very less characters: <https://startingwithsecurity.com/>.***

   4. ***I go through the entire application understanding the functionality and business logic. Mean while I keep inserting general XSS payload with my burp crawling everything at behind. Then I look for access control-related issues. Later in the burp sitemap, I place everything into the repeater and look for injection-related issues. Where I take the help of some automation as well.***

   5. ***I would suggest learning about each functionality a website or an app provides. Once you learn that you will have an idea what should *not* happen. And then you make that happen and you have a bug.***

   6. ***I have <https://www.wappalyzer.com>. The plugin pretty well enumerate all the software used. And then I just google for a CVE, or if it is an open project on Github, I look for public issues filed.***

   7. ***Well, I feel Twitter is the best place as every zero-day goes vial here. Rest you can check in exploit DB and other platforms which store a DB of CVE's. It not very likely that you will find an exploit there. But you can always reverse it with the hints.***

<br>

 - How to bypass CORS filter and exploit for High Impact?

   - ***You can look for misconfiguration due to improper regex. Like http://abc.xyz.evil.com or look for whitelisted domains and its bypasses. I would suggest to go though this blog of GeekBoy: <https://geekboy.ninja/blog/exploiting-misconfigured-cors-cross-origin-resource-sharing/> & <https://geekboy.ninja/blog/tag/cors-exploitation/?sfw=pass1619678376>.***

   - ***For high impact. You need to what data you access via the misconfigured CORS. Remember, CORS is misconfigured only if it can access private data. CORS set to "\*" on a public endpoint is not a vulnerability.***

<br>

 - Can you please tell us about your cobalt core recruitment process?

   - ***I was among the very early joiners. Like 4 years back when they started this pentest programs. A lot of things have changed after that. All I can suggest is they look for people with industry experience and professionalism.***

   - ***And you should know about all the bugs rather than being a crit hero or just a bug-bounty hunter.***

<br>

 - Q1) Any tips on Time management?

 - Q2) Any tips on Stress control tips?

 - Q3) Who's your inspiration in this field?

 - Q4) You are an ex-security analyst and what was the interview process and do you remember any questions asked in the interview?

   1. ***Being a product of Army school. I was good at time management. While I was in college. I bought a printer and I used to print reading material so I can study them during the classes. Most professors would go mad if you use your phone. No one objected to a printed paper. I have no streaming policy. I don't watch nextflix/youtube and all. Only with family. That too I keep an eye on the time. When I work I work. I prefer to get a job done asap. And then spend rest of the time with family and friends. Please note a break is important. We need to understand sitting all time on computers is not productive. It is equivalent to keeping a book open and not reading. So ideally you are not learning and you are not even having a break/fun. Take breaks, & when you come back, hunt seriously without distractions.***

   2. ***Always remember everyone had different circumstances and abilities. So don't compare. Be happy with what you have and what you did and keep improving. Not everyone needs to be a million-dollar hacker to be happy. You can be happy with few bucks and be with your family.***

   3. ***I was inspired by [@fb1h2s](https://twitter.com/fb1h2s), [@SandeepL337](https://twitter.com/SandeepL337) whose name I found in google hall of fame. Later on, I found [@ITSecurityguard](https://twitter.com/ITSecurityguard), [@fransrosen](https://twitter.com/fransrosen), [@NahamSec](https://twitter.com/NahamSec) Nir gold, and many others.***

   4. ***The interview process was very straightforward. There was an HR round technical round and one live triage round. You need to be an all-rounder here. Be good with communication as well as technical skills. Your concepts of all types of bugs should be clear. And CVSS scoring. For CVSS scoring I would suggest the free course of <https://first.org/cvss/>.***

<br>

 - How to get into web security? Can you suggest any specific learning way or the ways that worked for you?

   - ***Understand how web applications work:***

   - ***For this, I will suggest learning basic programming. Make sure when you are learning all the integrations. What common mistake I have seen new learners doing is they learn frontend separate, backend separate, database separate. Please don't do this. Learn everything HTML js PHP/node MySQL/mongo whatever you wish and then learn to integrate them all. It can be done by writing a simple CMS or a dynamic website.***

   - ***The second step would be to learn about web vulnerabilities. For this, I would suggest reading bug bounty writeups, play CTFs. A great book to start with is "The web hackers handbook". Check this out: <https://startingwithsecurity.com>. This should answer all your questions.***

   - ***The final step is persiatnce. Your fist bug may take months to come. But it is like a rolling stone. Once you find your first bug, you will keep finding it, and the key is not to give up.***

<br>

 - What were some of your favorite writeups that truly taught you something you didn't know?

   - ***I believe all writeups are important. Try not to miss any of them. The idea behind it is that when you are looking for bugs, your brain will remind you that you are in the same scenario related to a writeup you read somewhere. I would suggest this -> <http://h1.nobbd.de>.***

   - ***Also, I have been a fan of <https://labs.detectify.com/tag/frans-rosen/> and [@NahamSec](https://twitter.com/NahamSec).***

<br>

 - Q1) How you started as a beginner in bug bounty?

 - Q2) How was your setup (in laptop or pc) back than & don't you have neck pain on that?

 - Q3) Which bugs you find most and one can master/learn?

   1. ***I never started in bug bounty. I learned web application hacking out of interest. After a year I heard about bug bounties and tried my luck.  In 2013 I found my first bug in google and Paypal. They were both XSS.***

   2. ***Initially when I started I used to do it on my Nokia 5233. I remember I managed to inject SQLi through it. One of bug on dropbox was also via phone. It was an XSS. That time dropbox was not on HackerOne: <https://dropbox.com/special_thanks>. Later on, I got a laptop.***

   3. ***Although I recommend learning everything. However, I find access control bugs very interesting. You can always find them if you learn the application logic very well. I am not much of a recon guy. I prefer to find bugs in the main application and the APIs. They are overlooked!***

<br>

 - What are some crucial tips to master server-side bugs? And your ways/methods to approach a web app for finding SSRFs and RCEs?

   - ***To master server-side vulnerabilities first I would suggest having some developer experience. You get a better picture as most of the bug bounty programs are blackbox. Portswigger labs are really great: <https://portswigger.net/web-security/all-labs>.***

   - ***Regarding your actual question. What I do is fuzz (<https://github.com/swisskyrepo/PayloadsAllTheThings>) all the parameters in burp after I have visited all the features. I send each request to the repeater and try adding some garbage values. The errors are really helpful in smelling a bug.***

<br>

 - I have recently started to learn Bugbounty I am solving labs in [@RealTryHackMe](https://twitter.com/RealTryHackMe) and [@PortSwiggerRes](https://twitter.com/PortSwiggerRes). Can you please say what you use to do when u started in Bugbounty and also what are the bugs as a beginner I should focus more on?

   - ***Honestly, when I started, there was no such great CTF and labs. It was way back in 2011ish.However, I later did a few of these labs and found them great. What I would suggest is just don't play the labs. Do real hunting as well. Learning is fine but you need to apply as well.***

<br>

 - Which stuff will you mostly prefer for beginners who are interested in bug bounty?

   - ***For beginners, I would suggest getting the basics of web programming. And then jump into web hacking. This is a very common question I get, so I have compiled a list here: <https://startingwithsecurity.com>. Do give it a read.***

<br>

 - How did you land a job at hackerone? As I am also trying to get an infosec job.

   - ***I saw the job posting on Twitter and sent my CV and cover letter. Keep an eye on that. Also, LinkedIn is a great place to look for jobs. One more way is to go to a company's career page and maybe just shoot an email. Whats worse? They won't respond.***

<br>

 - What is required to work at Hackerone as a security analyst? Can I apply with a web experience only?

   - ***Yes, you can. The skills required are very well mentioned on their official website (under security analyst) <https://hackerone.com/careers>. In short, I would say apart from technical skills you need to have good communication skills.***

<br>

 - Tell me about your subdomains gathering/enumeration methodologies.

   - ***I not much of a hardcore recon guy. I spend most of the time looking for bugs inside the application by understanding the application and the business logics.*** 

   - ***For subdomain gathering I use Jason's bug hunter's methodology and some sort of self automation: <https://www.youtube.com/watch?time_continue=6&v=p4JgIu1mceI&feature=emb_logo>.***

<br>

 - What wrong things you have done when you were beginner?
 
   - ***I used automated scanners and reported bugs without understanding. That was like 8-9 years back.***

   - ***I will say semi-automation is effective. You automated stuff which is repeating rather than completely relying on someone else tool. And automate logic but learning the logic and concept is more important.***

<br>

 - Any weird bug you reported which you are proud of?

   - ***I noticed facebook started a conference website, fbf8(I guess, it was in 2017). I tried to log in using a random password with an internal email, and I was logged in. Later I realized any password would work if you are using an internal email.***
