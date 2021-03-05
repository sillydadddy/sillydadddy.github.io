---
layout: post
title:  "Infosec Bugbounty AMA with RougeSMG"
categories: infosec-bugbounty-ama
excerpt : "AMA with RougeSMG"
author: Gurvinder Singh
---

# AMA with [RougeSMG](https://twitter.com/RogueSMG)

<br>

 - Can you tell me how to find sql injection and other injection vulnerability and which parameters to look for? Also, how much time should we give to bug hunting and learning like the ratio of hunt:learn?

   - ***There's no secret trick. Our lives are filled with trial and errors! You'll gain more ideas as you keep hacking. It's like playing any game. The more you play, the more you understand the villains, your own character and the controls. And the better you get gf patterns by [@1ndianl33t](https://twitter.com/1ndianl33t) is good enough start to find potential params.*** 

   - ***Learning is very important. There's shit ton of new Bypasses and techniques being released everyday, you gotta stay updated. But remember, practical hands on >>> theory, so get some basics and go hack!***

<br>

 - I almost hit 11 months in bug bounty hunting field without finding any valid bug, I just wanna ask you how to stick hunting on single program I can't do it I don't know why I didn't find a program I AM comfortable with!?

   - ***The main issue imo is not sticking to a single program. And agreed, it's hard at times to stick but do it and it'll be worth it. Try this:***

	   1. ***Pick Dell/Sony.***

	   2. ***Get the subs.***

	   3. ***SS or look manually.***

	   4. ***Pick a sub with many functions and hack for 15 days at least.***

<br>

 - Any weird bug you reported which you are proud of?

   - ***Yes, it was on Pentest Engagement:***

	   1. ***Role based app with Rest APIs.***

	   2. ***Tried accessing High Priv user functions with Sub user tokens on all endpoints - *401/403 Denied*.***

	   3. ***Changed endpoints from:*** 

		        ***"/profile/changexyz" -->***

				***"/profile/changexyz/"***

	   4. ***200 OK - Privilege Escalation on all endpoints (PUT/POST).***

<br>

 - As a CTF player, what are some common mistakes new CTF players regularly make?

   - ***It's been quite some time since I played CTFs. But the most common issue is that people tend to forget CTFs are about learning and not just scoring. Actually try to understand what's the bug and the exploit and not just read similar stuff and blindly focus on the flags!***

<br>

 - What is your apporach in .js file in bughunting and What is your approach in github recon?

   - ***For Js: <https://twitter.com/RogueSMG/status/1350793896175886339?s=19>***

   - ***I don't do much GitHub recon but whatever I do it's all manual. For some deep insights Videos on my channel might help: <https://www.youtube.com/channel/UC855OCrjl7C3elK8VfEZoHw>.***

<br>

 - Q1. What skills do i need most before getting into bug hunting?

 - Q2. What should i focus on after clearing the basics?
 
 - Q3. Should i start bug hunting with beginner level knowledge or should i develop more skills and then get into bug hunting?

	 1. ***How the web works. Cookies, tokens, urls, servers, cache, etc. Get down the basics and rest you'll learn along the way.***

	 2. ***Practice on labs to gain confidence --> vdps --> bbp.***

	 3. ***Learning never stops. Just start and you'll learn more along the way!***

<br>

 - Tips to get started in CTFs? Also, how to find PoCs for CVEs?

   - ***Focus on the learning part and not just the flags. You can start w no knowledge at all, you'll learn a lot along the way!***

   - ***Google. For the ones that don't have a publicly available PoC, honestly idk but I guess your best bet would be to try exploiting it yourself!***

<br>

 - Could you suggest some beginner friendly CTF platforms please?

   - ***You could look on [CTFTime](http://ctftime.org) or on twitter for upcoming CTFs. [Hacker101](http://Hacker101.com) is a great one too!***

<br>

 - How to find information disclosure bugs in js file?

   - ***Ctrl + F and some tools like Linkfinder, jsscanner, etc. Main aim is to look for hard-coded stuff: api keys? Db creds? Internal creds? Sensitive information wrt the organisation? - Eg. If Healthcare, patient details, etc. Next, try to understand what the code does. Loopholes=win!***

<br>

 - What you do with default pages and that domains have login functionality and nothing else?

   - ***Dirbrute/ffuf.***

   - ***Login on that domain and try to open and look/brute other subs with those cookies for Info Disclosure or other interesting\* stuff that might pop.***

<br>

 - How to find SSRF and where to look?

   - ***Look out for parameters or functionalities that seem to be interacting with some internal service or dealing with URLs. Webhooks for example. And for parameters, redir, url, next, location, etc. sounds worthy. Sometimes, it might be fruitful to try it via the Referer Header.***

   - ***Try accessing Localhost, internal IPs, Cloud Service IPs (aws, azure, etc), Protocols life ftp, file, gopher, etc. Maybe some bypasses for those if restricted. Google is your friend.***

<br>

 - Which scope you like to hunt on?

   - ***Medium sized scope, not too huge.***

   - ***Some Active recon - Dorking, and finding an interesting\* subdomain and dive deep into it. You can watch the videos on my channel for some more insights: <https://www.youtube.com/channel/UC855OCrjl7C3elK8VfEZoHw>.***
