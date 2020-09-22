---
layout: post
title:  "Infosec/Bugbounty  AMA with AnugrahSR"
categories: infosec-bugbounty-ama
---

# AMA with [AnugrahSR](https://twitter.com/cyph3r_asr)
He is a very hard working beginner in #bugbounty , He just finished #100daystolearnandimprove, Lets learn what a beginner learnt in 100 days.
<br>
# About AnugrahSR 😎  and His Journey💪
- How hard it had been for you to enter from a diff sector to this bb? what is the reason behind your interest in bb? and tell your story.
 

  - ***I'm a trained biologist(masters)Upside-down face during one of my summer research internship, I was away from friends, loney& depressed, for time killing I got into social media with a fake alias and learnt about some cool hacking stuffs such as SQL injection, shelling etc.One day saw people Posting their achievements in bugbounty such as swags, hof, mugs ,sony t-shirts. Tried to contact some people, no one really helped and there was no such community support back then in 2017 I guess. I went back to normal College stuffs.Then when this covid kicked us out of college and sitting at home scrolling through Twitter I found my old followers list with security researchers. I found @aish_kendle doing this amazing challenge, and I looked at his progress and process and eventually jumped in.Having my knowledge in computational biology, I had some skills in bash and reading codes. I knew almost all the owasp top 10 and what it do. It was hard to pick one and learn. I found 
 @harshbothra_ talk's as a eye-opener and source of motivation.One thing I learnt in twitter is that, there is a button to know what others people liked.Just go and spy on the researcher you will get more amazing peoples, write-up, tools.
 Ifs someone post a bounty post, track down the company and hack, gey bounty.
 Small goal setting are good***


- What is your first reward in this journey and how much time it take you to find your first vulnerability.
 
  - ***Accenture hof after 2 weeks of starting will be my favourite, learnt a lot in that rdp prgm! huge scope, subdomain enumeration, directory brute-forcing, screenshotting and more***

- How long have you been hunting? And how many programs do you focus on?
 
  - ***I have focused more on public and private vdp prgms with large scope. I have tried with responsible disclosure, I haven't got many replies so just went with bugcowd. I have been hunting for last 3-4 months.***

- What are the vulnerabilities you hunt for everytime and you mastered ?

  - ***I haven't mastered any vulanarabilty class to be honest, but most of the things I look for are in this amazing repo by 
 [@KathanP19](https://github.com/KathanP19/HowToHunt)
 I have got good at expanding my attack surface for now. Goal is to master a functionality abuse or bug type.***

- Favorite recon tool ??

  - ***Osmedues and nuclie***

- Please write a write-up or blog about what you learnt in this 100 day also include what knowledge you had then and after the challenge what knowledge you have. what things you learn and what challenges you face
  - ***Working on writting my first blog, mostly with in days it will be published.Here the blog [AnugrahSR](http://anugrahsr.me/)***

- How you were introduced to bug bounties bro? (Where did u hear about bug bounty at first time) and what was your first thought that came to mind after hearing so..
  - ***Introduction to bugbounty, saw people posting intel acknowledgment, sony t-shirts, mugs, hof in 2017. Followed bunch of people's in tweeter, asked a few and no one really helped that time. In lockdown I saw the people I follow back then posting videos, tutorials, write ups***
  
  # Tips For Recon 🔍

- Steps for recon..?

  - ***It's have almost all the things I do. Sometimes I just skips things and just collect subdomain and run scanners to get easy stuffs.
 Mindmap taken from [Rohit Gautham](https://youtu.be/z24ELkocsJE)***

- After all the recon, how do you find that "Yeah! I must start with this"?
 
  - ***What I usually do is, get a list of subdomains, screenshot it. If it have a login panel or seems interesting will look at that.Or take subs one by one and run ffuf. I have got into unauthendicated admin panels like this. Then check for rate limits, password reset, auth misconfig***


- Do you perform directory brute force in your recon methodology? If yes, when do you feel like ‘yeah now I’ve to perform directory brute force on this endpoint’ ?
 
  - ***When I have a list of subdomains, I usually screenshot websites with aquatone and open each websites and run ffuf or dirseach on that. Running directory bruteforce have allowed me to find simple phpinfo files to access to admin panel. I want to try making custom wordlist oneday***

 
- What wordlist you use for ffuf permutations subdomain bruteforcing

  - ***Subdomin bruteforce: I use commonspeak + all.txt Permutations.I use the buildin wordlist itself in altdns or dnsgen.Dirseach generic wordlist***
  
  # Resources For Beginners 👨‍🎓

- What are some good resources to go wit if you have zero knowledge into wapt or you say bug bounty. Any github pages, websites, books, vm's, videos, courses and any or many things which you can say. Thank you   
 
  - ***Read this write-up by 
 @udit_thakkur
 3-4 times, you will know where to start and what to do. Best get starter guide out there. Sorry for the delayed response, I didn't see this question
 https://medium.com/hackcura/learning-path-for-bug-bounty-6173557662a7***

- When you learning a P4 bugs what methodology  you followed bro...
Ex:Choosing a  bug..

  - ***Best place would be [bugcowd vrt](https://bugcrowd.com/vulnerability-rating-taxonomy)
 Take a bug, search on google read reports, watch poc videos and try it on targets.
 This repo have almost have some [Good methodology]
 (https://github.com/KathanP19/HowToHunt)***

- How did you manage your time..?

  - ***I'm really bad at time management, I get carried out when I see somthing interest me. Still reading blogs and watching videos, looking at tweets and all of the sudden I get feeling to hunt on target, I do it when I'm comfortable, that why whenever I hunt I found somthing.2hr reading + 2hr hunting would be great. Daily 2hr reading blogs or tutorials will be a great practice***

- Which wordlist you use for directory bruteforcing?
 
  - ***Jhadix wordlist***

- What is your methodology for hunting bugs..
   
  - ***I follow this methodology, project bheem mainly with minor changes of mine.***

- Where can I get POC and other blogs about old exploits :)
  
  - ***can't point you anyplace, you can find some exploits in GitHub, some in google hacking database, some blogs. Google-fu skills is the answer for this.***

# Burnouts 🔥

- During your 100 days of improvement how many burnout you faces !
 
  - ***More than i thought, aug was one among them, didn't do anything than watch youtube videos and tutorials. Rest of the times I was able to get back within weeks of time.
    Having people around you to talk to is great, writting bash scripts was my way to overcome***
