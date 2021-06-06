---
layout: post
title:  "Infosec Bugbounty AMA with Akita"
categories: infosec-bugbounty-ama
excerpt : "AMA with Akita"
author: Gurvinder Singh
---

# AMA with [Akita](https://twitter.com/akita_zen)

<br>

 - Q1) Is there any important things you think one should keep in his mind before picking a taget?

 - Q2) What suggestions you will give to your youngerself who is struggling to get the first bounty?

   1. ***Choose any Owasp Top 10, then look for hacktivity about that bug & try to replicate. This need to be fun, so choose wisely that bug & play a little. Then just dive on any program & hunt! Persistence is key, so if you fail, you need to understand that fail is just training. Try harder until you get bounties!***

   2. ***Fail after fail is the real success. Go for it & you will get a bounty very soon!***

<br>

 - What’s your strategy to recover after getting burned out? How do you still keep finding cool bugs even after coming from long breaks?

   - ***When the mental activity stops at rest, everything clears up, this implies taking a time away from the overactivity that the bb generates, then when you return, your mind is fresher and you can see/perceive more, the mind is awake, since it does not contain the daily noise that the bugbounty generates, if this daily noise is not controlled can leads to burnout.***

   - ***An urgency plan to recover burnout:highly suggest: close your laptop,put a mask & go outside (or look for an inner garden)mind need to rest & frequency nature is his root connection(barefoot & grounded)to release all stress accumulated in body,feeling your conscious breathing.***

   - ***Anything that works for you that leads to a "shift" in your energy field, mental, emotional, physically. Sports, yoga, martial arts. Anything that works for you will be fine,one principle to follow is that body/mind are a mirror,so if you move your body,you are moving your mind too.***

<br>

 - Do you have your own checklist for testing? What learning resources do you follow regularly to upgrade yourself? Did you ever got any job/internship offer from any bug bounty program?

   - ***Yes, I get some offers in the past, but I rejected all them because I'm a person which has troubles having a work schedules, hours, etc. Thats why Bugbounty fit perfects in my lifestyle.***

   - ***Not checklist here. Just going through manual until I see something that call my attention and dive on it.***

   - ***Resources: mostly Twitter writeups, following good hunters. Newsletters, hacktivity, Github, etc.***

<br>

 - When you were starting out, how did you cope up with burnouts and low motivation despite trying hard to find vulnerabilities?

   - ***At some point I forget about bounties & just was over learning Path because was/is fun. Sometimes I forget about this(time to time I need to remember myself this again)About burnout, when you loose so much health (mental, physically)You take it very seriously & it's priority.***

<br>

 - Do you know any good resources to find breached credentials?

   - ***Watch this video: <https://www.youtube.com/watch?v=l0YsEk_59fQ>.***

<br>

 - What is your go to vulnerability, the one you always start in any bug bounty testing?

   - ***I Love Authentication Bugs (Mostly SSO -> SAML, Oauth, openID, etc) & Server Side (SSRF mostly!).***

<br>

 - What is that (hacker)advice that you would give to your youngerself?

   - ***Always comeback to the basics, develop the beginner's mind, if something put to serious just let go & have fun doing Bug Bounties. Enjoy the Game, Enjoy Your life! Don't be anything for granted, keep your mind always open & flow with the wave.***

<br>

 - Q1) Does joining IT faculty will help me in bug bounty career or red team career?

 - Q2) How do I start in bug bounty? I still learn the basics and got bored from time to time asking myself am I doing it wrong or what? 

 - Q3) Can you tell me the way from start to at least taking my first program?

   1. ***Any knowledge that you can add as "skills" will help you to achieve great things! IT career, a certification, etc. The most important thing is that you enjoy doing it, finding and looking bugs, seems like a treasure game.***

   2. ***When I started Bug Bounty Hunting, I had a lot of months failing, so that's normal process, don't give up & keep trying. Resources are everywhere: from great write ups, amazing hands on labs ([@PentesterLab](https://twitter.com/PentesterLab)), daily newsletters ([@intigriti](https://twitter.com/intigriti)), [@Hacker0x01](https://twitter.com/Hacker0x01) or [@Bugcrowd](https://twitter.com/Bugcrowd) hacktivity.***

   3. ***Take 1 bug from hacktivity or write up & try to replicate in other programs, this is great to get your first valid bugs/kudos/payouts and great motivational engine to keep digging, learning and going beyond!***

<br>

 - Which bug you find the most and how one can find them?

   - ***Mostly are chains of different bugs like SSRF (Privlege Escalation) or authentication bypass. All documented in public write ups! (Nothing fancy, maybe kind creative attacks)take a look to program documentation,take your time doing the right recon(Even if take days, weeks or months).***

<br>

 - What weird cases you found on these scenarios: Authentication related, OAuth related, SSO Related?

   - ***[@PentesterLab](https://twitter.com/PentesterLab) pro Authorization Badge, its amazing (mostly of Oauth, SAML, Auth scenarios are similar to all of those you have on bug bounty programs).***

<br>

 - Can you point out some instances in your Bug Bounty career, wherein reading docs had been really fruitful to you?

   - ***Mostly was focusing over API documentation, you will find potential hidden endpoints (dev/staging/qa) that can works on production! Also gives you an idea of how is implemented the app frontend & backend API.***

<br>

 - Why & how you hack?

   - ***Why? Because it is fun & I'm a very curious guy from that I was born!***

   - ***How? Training like a ninja, every day learn something new and acquire a new skill!***

<br>

 - Can we apply the same Top 10 Owasp Technique for (Application/Json) data which we usually approach for which are not based on API? Normally most of the bug bounty program where I test security are in text/html format where I test for Top 10 OWASP, like Injection attack and other things. But I recently met some program which uses API( Application/json) content type. So I want to know If I can apply?

   - ***If you come across with these scenarios where Content-Type: application/json you can test for specific vulnerabilities, from sql injection, 2fa bypass, IDOR: (private escalation -> user to admin) like crafting the response {"failure"} -> to {"success"} changing response code -> 401, 403 to 200 OK, etc. Always do a recon of the backend as much as you can, like what framework is used, a wide recon of the app, etc.***

   - ***{"role":"user"} -> {"role":"admin"} etc. And You can achieve too XSS! , because sometimes application relies on a backend API with Content-Type: application/json, but in the frontend you get text/html, so payload Injection works and popup in the app!***

<br>

 - Suppose I have to Inject Sql Blind payloads here:
 - Normal request - 
   ```
   {

    "email":"test@gmail.com"

   }
   ```
 - Sqli Injected request - 
   ```
   {

    "email":"test@gmail.com' sleep (10) --"

   }
   ```
 - I'll have to Inject like this right?
 
   - ***Yes, indeed you can take a list of sql injection payloads and FUZZ IT! but remember that blinds are hard to get! so you need to use error handling like time responses, etc,  to blindly knows if sql injection is really done there!***

   - ***Another great way to do this is with sqlmap or burp extension. Sqlmap is an amazing tool when is used properly!***

<br>

 - Suppose I inject payload and the response I get is 422 unprocessed entity. What should I do in this case? Ignore it or just play with that around using some bypass techniques?

   - ***There are too many different factors! what I do in this cases is look for some write ups which have a similar scenarios and try those things, sometimes you never know what can happens! Even with 422 you can achieve XXE if CT is xml!***

<br>

 - Q1) What are your views on these bug bounty courses released almost daily by some other hacker these days?

 - Q2) Do you use any paid services in your bug bounty workflow? If yes, then can you name them?

   1. ***I'm a big fan of free/public resources! about that courses, maybe can be useful as starting point to get a general idea about Owasp ToP 10, etc. This is great way to start with free resources -> <https://twitter.com/stokfredrik/status/1399633125123239936?s=20> [@stokfredrik](https://twitter.com/stokfredrik).***

   2. ***I use Shodan as membership (one unique payment of $49) is quite limited but for me is enough to search what I need. I have too [@PentesterLab](https://twitter.com/PentesterLab) Pro, which is one of the bests places to learn web hacking/pentesting! Totally recommended!***

<br>

 - What's your opinion about CTFs, Tryhackme or Hackthebox machines?

   - ***I dont have real experience on those, however CTF is kinda fun and p0wing boxes too! Maybe are more close yo "Pentesting" that bugbounty, achieve an RCE or play with internal networking deeper is not a daily thing on Bug Bounty scenarios.***

<br>

 - I am beginner in bug hunting but I see that all common bugs are already fixed then how can I find bugs? Any guidance?

   - ***Look for a different approach, try to understand the lógic behind what You are testing. Create your own methodology & go deeper when testing a program, not only on the Surface, Even if take weeks, keep learning and doing an strong recon.***

   - ***Take a look at this [@stokfredrik](https://twitter.com/stokfredrik) gem!: <https://www.youtube.com/watch?v=SBCpfYFs610>.***

<br>

 - You are one of my inspirations about building a mindset to "don't do the same". What made you think like that? What you usually do to keep you "dont doing the same"?

   - ***My lack of skills force me to think different is so many ways, because when you can't go further to known attacks vectors, you need to put your mind in "creative" mode, and that's how I avoid dups too!***

   - ***What I do is looking for different approach than the common tested like automation of tools and one-liner commands, etc. (because all are doing the same) So think in terms of impact & go to borderline of the scope from outside to inside until you hit the best impact of app/site.***

<br>

 - How many hours do you (Hack/Sleep/Twitter/Read) daily?

   - ***I'm back recently from 9 months off bb to improve My health, right now very little Activity, (only 3 reports on may = 5 days = 8 hours daily) but most of the time maybe 4,5 hours/Day, 4 days a week.***

   - ***I wish to read more write ups & do more labs, but health is priority, so my yoga, Tai chi and daily sports are always first.***

<br>

 - Where to apply the concepts that we learned from PentesterLabs?

   - ***Indeed in this days, I still found bugs in public programs already over tested! so remember that your view always is unique, give a shot! Directly on the Bug Bounty programs! Dive on it!***

<br>

 - What's your approach from start to end to find bugs in target, like tool for sub enum > param fuzz > content discovery? At what point of this process you start looking for bugs manually?

   - ***I start with .*\.domain\.com$ over burp and hit a wide scan, view report issues, endpoints, requests, responses -> if something get my attention I deep on it manually & if its necessary I run some tool from terminal like ffuf to FUZZ or some burp extensions!***

   - ***About which issues like to hit are Server Side bugs (mostly SSRF) so I use parameter <https://github.com/PortSwigger/param-miner> or something related tool & for Authentication looking every request/ response flow to find issues like Oauth, SAML, OpenID, etc.***

<br>

 - What is your approach when doing bug bounty, selecting one program and hunting for it until finding a bug or selecting more than one program and switching between them?

   - ***I hunt on 2/3 programs only because I know those environments(a lot of time invested on those). About new programs,I use burp & do a wide scope scan to see a general aspect of it & then go manually/deeper over something thats calls my attention, always looking the best/big impact.***

<br>

 - What usually you look on vulnerable end points, is it depence on what programming language and framework, or private user data or anything else?

   - ***Mostly weird behaviors on the site/app/api, request/responses, framework backend, error handling. This is a good resource for params based on gf tool: <https://github.com/1ndianl33t/Gf-Patterns>.***

<br>  

 - What's your fav bug and highest $ you earned from 1 bug?

   - ***I love Server Side & Authentication Bugs! My highest payout was an RCE (1 bug) US $13150!***

<br>

 - Would you recommend a beginner to go for IDORs Or XSS?

   - ***Totally! Those Bugs don't require expertise knowledge! Those are all over the place! Just dive on it!***

<br>

 - According to you, what is the error that most new hunters make?

   - ***Doing the same as others, looking the same as others. We can see this a Lot on Surface recon automation, oneliner commands, same tools used un same places, etc.***

   - ***Don't get me wrong here: is not bad try things and learn from them, but at some point if you want different results, you cannot achieve this doing the same things as others! Thats why its really important that with time create your own way to think! your own methodology!***

<br>

 - What do you prefer the most: Client Side or Server Side Bugs?

   - ***Now Server Side Bugs, but client side are really great & love them play & be fun.***

<br>

 - Can you suggest me a good platform to apply my learning which gives me a real website ideas?

   - ***[@WebSecAcademy](https://twitter.com/WebSecAcademy) great labs!***

<br>

#### The original twitter AMA can be found here :- <https://twitter.com/sillydadddy/status/1399498091196080130>
