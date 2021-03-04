---
layout: post
title:  "Infosec Bugbounty AMA with Sajeeb Lohani"
categories: infosec-bugbounty-ama
excerpt : "AMA with Sajeeb Lohani"
author: Gurvinder Singh
---

# AMA with [Sajeeb Lohani](https://twitter.com/sml555_)

<br>

 - What CVE are you most proud of?

   - ***Ooo! Tough question! My most widespread one was probably a privilege escalation bug in install4j's uninstaller. It is used in software like OWASP ZAP and BurpSuite.***

   - ***Also, a shoutout to the OWASP ZAP team for helping me figure that one out. I found the bug in their uninstaller but never would've known how widespread it was without them telling me!***

<br>

 - How to avoid crowding in bugbounty?

   - ***Hunt where no one else is looking, or know the bugs you look for better than anyone else. Frankly, overcrowding of a target is inevitable, so get in early and hunt as best you can. Try to go beyond the normal tooling everyone talks about to uncover new unknown assets!***

<br>

 - Which vulnerabilities we need to focus on avoid crowding, can you share?

   - ***Business logic issues and issues specific to applications are less likely to be duplicates imo. It's really hard to say, but whenever you dive into an application, and look at functionality which others like haven't (like paid functionality), you increase your chances of success. Thanks to [@stokfredrik](https://twitter.com/stokfredrik) for that trick btw!***

<br>

 - 1. What is the future of bug bounty?
 
   2. I wanted to do full time bug bounty after 12 so will it be a good decision?
 
   3. What is the importance of maths in cyber security?

   4. What is the chances of getting a job if we do bug bounty as a full time without collage degree?

   - ***1. That's a really tough question. There are plenty of areas bug bounties can grow. I'm sure different companies will take different approaches, so I'm keen to see where it grows too! Over the past few years, the growth of rewards has been great and I'm sure people will be opening up to larger scopes in the future too!***

   - ***2. I assume you are asking about year 12 here. I'd actually recommend studying further and keeping bounties as a side-gig. (This may differ based on other factors like geographic location). Having a degree and being able to fall back on it, incase something goes wrong is quite necessary (imo). At least it is worth have a think about.***

   - ***3. This depends on the level of maths you are talking about. All of us need to have the ability to count our money and budget, in order to live our lives properly. That can be considered basic maths. Estimating things like timing can also be a good usage of maths in technical security. Finally, the scariest one is cryptography. This likely requires the most mathematical skills (imo).***

   - ***4. That is really hard to say. This really depends on your location and the skill set you bring. When you are going for a job, remember to try answer the question, "What do you bring to the company?". In some cases, crazy technical skills are exactly what they want, which counts as a big plus for you (provided that is the type of hunting you were doing). The idea of a college degree is that it provides a level of assurance for your knowledge and ability to learn. So it is still worth considering, but really depends on your specific situation.***

<br>

 - I'm really impressed with the amount of CVEs you have under your name. How did you get these? Cause you need a very... Different approach to things before you can even get a CVE. How do you analyze things? What do you look for? What's your way of handling these things?

   - ***Glad to hear that! I enjoy reading a lot of code, so I spent a few years reading the code behind a bunch of open-source projects. I majorly focused on languages I knew relatively well (or wanted to learn better), like Python, Java, PHP, and C(learning better).***

   - ***There are a few things that you can do. 1: Look for specific issues that you are familiar with (like XSS everywhere) and then attempt to find it in a bunch of different projects, or, 2: understand how the application is built and then try to identify abuse scenarios.***

   - ***Number 2 tends to find scarier bugs.***

<br>

 - Do you have an approach to which companies you target? Or do you pick one at random and adapt to what you see?

   - ***Monash has an awesome team with Dan Maslin, but they are a good target to hunt bugs on (provided you have the invite and permission).***

<br>

 - Did you find bugs doing github recon? Shall we know about your methodology towards github recon? Some tips to win in github recon?

   - ***To be honest, I've only ever found 3 bugs with github recon. All three were P1 tier bugs, but 1 of them was a duplicate. I recommend following [@Th3G3nt3lman](https://twitter.com/Th3G3nt3lman), who made a video (<https://youtube.com/watch?v=l0YsEk_59fQ&t=1s&ab_channel=Bugcrowd>) talking about his github recon method. He's an absolute boss!***

   - ***In that case, I recommend trying to change things up a bit! Read tutorials and understand the thought process. Then apply your own experience and unique spin! That might help find new bugs which others haven't yet!***

<br>

 - How many programming languages you know and does it helped you in any means learning those Languages?

   - ***I think I know north of at least 10 languages well. After you have developed with a few key languages, it becomes much easier to learn new ones! Python, C, Lisp, and Java are examples of how languages can change a lot, but learning them can be helpful to learn others!***

<br>

 - Does your Programming skills helped you in finding CVEs?

   - ***Definitely! I'd actually say it is one of my biggest strengths. I was trained as a Software Engineer, but chose the line of security. It helps to not be afraid of code and helps uncover some really cool bugs using the context of the code.***

<br>

 - Learning php or any backend language is really helpful to find SSRF. And from where to start to hunt SSRF?

   - ***I'm assuming that you are asking whether findings learning a backend language like PHP can help with finding SSRF bugs. It can, however understanding how the networking side of things work will likely be more helpful! eg. 127.0.0.2 is still localhost, but may help bypass filters.***

   - ***[@PortSwigger](https://twitter.com/PortSwigger)'s Academy has some good resources to learn from too! I recommend taking a look at their challenges!***
 
   - ***If you are looking for more resources, [@PentesterLab](https://twitter.com/PentesterLab)'s pro subscription has some good challenges too!***

<br>

 - Can you give some advice for people trying to find bugs in Bugcrowd (not Bugcrowd programs)?

   - ***Dig deep into the platform. Learn how all the components work and how they can be misused. That's general advice for everything, but works well for the Bugcrowd application too.***

<br>

 - Imagine, as usual we got subdomains list, trying something like port scan and nuclei, but I need go to the next step, like perform fuzzing/shellcode as universal solution. I read about simplest fuzzer \`cat /dev/urandom | nc hostname port\` but did't get what to expect?

   - ***For that scenario, you would be listening for the output from the port to see if you cause any errors or determine certain types of interaction. That is a way of attacking a target, but I don't excel in using those methods.***

<br>

 - How do you unwind/decompress/recharge whenever you're feeling close to burnt out? Have any non-digital hobbies or other interests intersected well or helped with your success or methodology in your opinion?

   - ***That's a really good question! I spend a lot of time with family and friends. This includes things like playing games, shooting pool, watching movies, occasionally hiking, planning pranks, travelling, and other random activities. I work pretty hard and forget to take breaks.***

   - ***But I'm quite lucky that I have a family that supports me and reminds me to hit the brakes on my professional life from time to time! While these hobbies don't directly compliment my bug hunting, they give me the necessary break to let my mind run loose and come up with solutions.***

<br>

 - Do you use use \`msfvenom\` to prepare target specific payload and use reverse shell like \`cat reverse.txt | nc targethost port\`?

   - ***It really depends on what I am trying to attack. When relevant, I have leveraged msfvenom (why not?). But in cases, things like AVs get in the way, which is when you come up with your own creative solutions to make your exploits work!***

<br>

 - How to know if a particular asset has any bugs or not (asked by a noob begginer sorry if silly) and also any advice for noob begginers who has no technical background???

   - ***I think the best approach would be to establish a method of testing. Something like chapter 21 of the Web Application Hacker's Handbook would be good for that. Basically it is a process that you follow in attempts to find bugs and gather information. It is a decent starting place.***

   - ***Also, reading something like the tangled web can be helpful! It will help you understand how the web actually works and a lot fo the different components.***

<br>

 - I just wanna ask you I almost hit 11 months in bug bounty hunting field without finding any valid bug, I just wanna ask you how to stick hunting on single program I can't do it i don't know why I didn't find a program I am comfortable with!?

   - ***Hey bud! Sorry you haven't found anything yet, but definitely don't give up! I think taking notes is quite important. Note down all the information you gather and keep it in a consumable format.***

   - ***When you feel like you can't find anything else and have exhausted all options, I recommend switching to another program. Look for programs where others have had a lot of success. It can be perceived as a good indicator that there is more to be found! Good luck with hunting mate!***

<br>

 - Any tips for beginners?

   - ***Sure! As a beginner, I recommend doing a lot of reading and knowledge gathering. Basically, anything you touch, you should have the curiosity to find out how it works. Read books like "The Tangled Web". Next, learning a programming language won't hurt and is worth considering.***

   - ***Python can be very helpful! After that, I recommend reading a lot of security related resources like the Web Application Hacker's Handbook and practicing on some practical exercises like [@PentesterLab](https://twitter.com/PentesterLab) and [@PortSwigger](https://twitter.com/PortSwigger) Academy. They help convert theory to practical skills.***

   - ***Reading things like security-related blog posts and bounty finding write-ups is another method of gathering a great amount of information. Thoroughly recommend doing that as some of the other hunters have highlighted the method they used to find certain vulnerabilities.***

   - ***C++ can be helpful with a few different types of hacking. Firefox is written in C++ iirc, so you can do browser hacking. Also, if you are good with assembly, then binary exploitation might be a good avenue!***

   - ***I'd recommend identifying the type of hacking you are most  passionate about and that suits you best! I'd recommend reading up on a bunch of different types of hacking and seeing which utilise your skills and passions best.***

<br>

 - Do you have a checklist or things to look for while testing an application?

   - ***Not really. [@Jhaddix](https://twitter.com/Jhaddix) made an awesome checklist over here: <https://gist.github.com/jhaddix/6b777fb004768b388fefadf9175982ab>. You can use that checklist as a baseline and start developing your own from there! Good luck!***

<br>

 - What's the coolest bug you've found and how did you go about finding it?

   - ***I think the coolest bug I've ever found was an LFI that lead to RCE. Basically I had an LFI, but I had a WAF to battle and a restriction that the file being loaded needed to be .css. I couldn't find a way to upload a CSS file (restricted in all places).***

   - ***So I went to the support chat and tried uploading attachments. Turns out I could upload ZIP files! I put shell.css in a zip file (with PHP code in the CSS file) and then used the zip protocol (zip://) to unarchive the zip file in runtime and include my CSS file (with PHP code).***

   - ***That lead to RCE! It took me another hour to priv esc on the server, leading to a full compromise. (This was on a pentest years ago).***

<br>

 - Do you look at the payouts while choosing a program?

   - ***Yeah, I definitely look at the payouts. If it is something low, then I likely won't spend time on it. Response time matters in some cases, but I don't pay too much attention to it, as I can wait for resolutions.***
