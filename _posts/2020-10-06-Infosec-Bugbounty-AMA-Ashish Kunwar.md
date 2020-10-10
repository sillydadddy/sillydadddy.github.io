---
layout: post
title:  "Infosec Bugbounty  AMA with Ashish Kunwar"
categories: infosec-bugbounty-ama
image:
  path: /images/DOrker.jfif
---

# AMA with [Ashish Kunwar](https://twitter.com/@D0rkerDevil)








- How did you get into hacking in the first place?
   
   ***Well, it all started 6-7 years ago when I was still in school and my city nagarpalika website got hacked and defaced by someone which really triggered me to how and why and that's where it all started***
 
<br>

- first bug you found? 
  
  ***First bug I found was in Malwarebytes and I got 100$ for it. I don't remember what the bug was but I did a write-up on my blog at http://dxploiter.blogspot.in***

<br>

- What prgm(not prvt) you will be hacking if you can only hack on one!

  ***I would be hacking on yahoo***

<br>

- What is your next goal in infosec?

  ***My next goal would be getting some certs and .... Will see how everything goes***

<br>

- faviourite tool and burp plugin?
   
   ***Fav tool @xer0dayz Sniper , there are many burp plugins but fav burp plugin  is logger++ and response clusterer***

<br>

- How do u use Burp suite ?
 
  ***Well i would suggest u to sit down and roam around the burpsuite and look which feature does what, u then don't meed to find that question cuz that's what I did ,u just need to spend some time with it***

<br>

- Any tips to increase the efficiency of Burp ?
  
  ***To increase efficiency in burp u can checkout how to efficiently use the burps scope feature and intruder***

<br>

- Which plugins do u find most useful ?
  
   ***I use logger ++ and response clusterer***

<br>

- What are the things you look before choosing a program?

   ***If they program says they will give reward which could be $$ ofcourse ,I don't go for swag  or just Hof cuz I have already tons of Hof and acknowledgements***

<br>

- How do you select which target to work on first and what do you see in the target?
   
   ***Already said , money is what I see if programs pays then m good to go But also the scope matter.If the scope has all their asset in scope then it will be the one m gonna spend my days with***

<br>

- what is your recon process ?

  ***I mostly do manually hunting cuz in automation I feel that I might some miss bugs which cannot be found with automation***

<br>

- How much of manual hunting do you do ?
  
  ***It's same as others subdomain enum > port scan > directory scan , etc***

<br>

- Do you use a VPN while doing manual bug hunting ?
  
  ***Mostly depends on the type of target I use vpn.***

<br>

- What is your way to approach bugs and can you provide the path / tips for a beginner to get into bugbounty
  
  ***Everyone has their own approach , mine depends on the target scope ,if the scope includes of the particular domain then I test right away , if the scope is consists of subs or acquitions then do subdomain enum and whois and all the essential things***

<br>

- @D0rkerDevil
 how do you do on public program? It seems people found a lot of things before you. How to do in this case?

   ***Well your have keep looking for what people miss , but it's not always the case if the programs is I overly tested then there is really low chance u gonna find anything, so move on to next***

<br>

- How to approach and recon  with a small scope program

  ***Depends if the scope tells u to stick to a single a single domains or any particular domains to test then, do as u usually do create account and start testing, couple of things u can do is look if there is any creds leak on GitHub or pastebin***

<br>

- How to hunt CVE-based bugs in applications?

   ***Simply Google with vuln version and u can find em atleast most of the time***

<br>

- Your methodology for pentesting mobile applications
  
  ***I do static analysis and look for particular strings that could be api keys or hardcoded creds ,etc and also I do use it with burp***

<br>

- Elaborate about your bug bounty setup e.g VPS, toolset, note keeping, checklist etc
  
  ***I use vps for most of the things like for recon and other stuff like fuzzing, for toolset it would be @xerosecurit Sn1per pro (do check it out) and few custom tools that I have developed for my needs , for not keeping I use notepad++ and similar , I don't have any checklist***

<br>

- how to hunt for cves
  
   ***With hunt for CVEs your mean looking for if the cve has been specified for particular application during BugBounty,then you can simply search on google like or look on cve mitre***

<br>

- Bro, what's your approach for finding bugs, exactly what you do when you choose a program such redbull Face with tears of joy.. How you find bugs in a one shot ?
  
   ***With huge scope like redbull I use Sn1per to grab subs and then look for open ports using nmap and do dirsearch on all of them and also filter the live subs using httprobe and look for them manually in browser, and I don't fimd bugs in one shot like others do.***

<br>

- One more doubt , bro is dirsearch should be used with default wordlists or custom target specific wordlists, as those words custom words already are paths, we got those paths using unfurl , jsparsing.. so how to curate these paths to find out new paths.. ??

  ***Crawl pages, use webarchive and also use jslinkfinder to find new path***

<br>

- Any tips regarding Automation ?
  
  ***use your own methodology and create something of your own***

<br>

- Hey Dude how u test for Blind SQLi ?? :)
  
   ***Tim based payloads and oobs***

<br>

- How do you modify your payloads for XSS? Also, is it hard to Bypass WAFs such as Cloudflare, etc?
Thanks in advance :)
  
  ***Look for reflections and how the web app modifies the response , I can then do bypasses based on that***

<br>

- What bugs can a beginner look for, and any resource to learn bug bounty or Web app testing
  
  ***There is no certain bugs , you have to use your creativity and open mindset to find issues.Start with owasp guide v4***

<br>

- When was first time u wanted to come to hacking, wht inspired u be in the field,wht tools do u preffer for sub domain enumeration

  ***It all started somewhere around 2014 , seeing others posting swags and bounties on fb around at that time. I use Sn1per heavily for my recon***

<br>

- How many bugs find without recon
 Ex.password reset
 Login releted bug
 Any other bug can find without recon

  ***u need to understand how the functionality works , just try to understand the flow and you will find the issues***

<br>

- What motivates you to hack
  
  ***You guys in the community but mostly I do it for the thrill cuz when u find the bug it will make ur adrenaline rush, the feeling of finding bug and then the cash u gonna make along side ofcourse the experience is what u get along side***

<br>

- How did you start off hacking?
  
  ***Seeing defaced sites I get amazed and that's what triggered me into hacking around 2014 or earlier***

<br>

- Why u hunt for 0days ??
  
  ***Why not , 0days are luv***

<br>

- hows the youtue channel planning goibg ib @D0rkerDevil

   ***It's just planning not start right away bud , I still have to look into other stuff but I will try my best to make it happen as I m really busy with exams and all***

<br>

- How to exploit if I find a cve? Exploit is not available on google and github also it is not there in hackerone reports(cve-2007-2379)
  
  ***well you have to grab the vulnerable source and play around with it***

<br>

- What challenges u faced when you are newbie to bug bounty hunting? 
N how did u overcome those?
  
  ***Well I didn't had anyone to guide me when I started, so what I did was my own , trial and error***

<br>

- What's the biggest mistake you made in bug bounty?
  
  ***Don't find vuln if the company doesn6ha e any BugBounty program or any kinds of security policy***

<br>

- On which type of bugs beginners should concentrate? And what is your favourite bug?
  
  ***Go for low hanging fruits***

<br>

- Tools that you use for recon purpose. And your favourite tool.

  ***Fav tools Sn1per and the tools @1ndianl33t
 created***

<br>

- How to really develop a workflow to find bugs?? rn I randomly try out stuff I find on Twitter and Google
  
  ***Same here , shhhhh.***
