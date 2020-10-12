---
layout: post
title:  "Infosec Bugbounty AMA with Sam Curry"
categories: infosec-bugbounty-ama
excerpt: " AMA with Sam Curry "
---
# AMA with [Sam Curry](https://twitter.com/samwcyo)

<br>

 - Give some tips for new bughunters

   - ***Find people to learn alongside if you can't find a mentor. Make it fun.*** 
   - ***Don't stress yourself about time invested or how fast you can complete something.***
   - ***There are no pre-requisites to hunt for bugs.***

<br>

- How u got into hacking ? What are the bugs you advice for me to look for ? and What are your fav. tools exp. Burp. If u wanna give an Advice to newbie bughunter whats that ?? (it should be unique) Btw Thanks 😍

   - ***Hey! - I got into hacking from the video game community. - Favorite bugs to look for are directory traversal and SSRF. - Favorite tool besides Burp is SQLmap - Start hacking as soon as possible Cheers***

<br>

 - I'm a Beginner and couldn't decide to choose either between Public Or Private programs, are Private programa more vulnerable or public programs more secure? Thanks in advance! And you are Amazing (as always :)

   - ***There really isn't a "more vulnerable" - if a program is public, they're likely more mature and are tested to be under public eye, whilst private programs may be more young/have specific expectations of the researchers. This does not really mean much for the actual codebase.***

<br>

- which specific bug type a beginner should look for

  - ***Cross Site Scripting. It's common, gives you an introduction to the client/server model and browser behavior, and gives immediate feedback (why is " turning into &quot;?). For server side issues, I'd check for SSRF/LFD/LFI. The parameters for these are often obvious (?url=).***
  
<br>

 - What os you suggest for beginners..?
Focusing on particular one bug  is good or focusing on all bugs is good..Which one is better..?
Can you share your recon methodology

   - ***Whatever you have experience using. Focusing on one is a good way to start, but I think everyone should eventually move to all bug classes/majority. See other replies for recon stuff :)***

<br>

- while learning about bugs what mistakes you made and what methodology you suggest to learn a bug ? Did Recon is neccessary to learn especially for beginners..? what is methodology while a hunting bugs..?

   - ***I made the mistake initially of depending on other people for things I could've learned myself and ended up digging myself into a hole when I went back to figure it out. Recon is not necessary but if you enjoy it then go for it. See other replies re: methodology :)***

<br>

 - What kind of vulnerabilities do you like to go for first?

   - ***Nothing in particular, to be honest. Just keep my eyes open for whatever fits the situation.***

<br>

 - what suggestion you give for beginners from your mistakes

   - ***When I first started bug bounty I'd sent a few dozen PMs and nobody had responded to me. I thought this was a bad thing, but I went out and studied things by myself and learned how to do the majority of work myself. I'd recommend not offloading the core learning.***


<br>

 - Best tool!
    
    - ***Absolutely Burp Suite. I don't use too many other things besides the plugins on the app itself.***

<br>

 - Burp plugins ?
  
    - ***JSON beautifier, param miner, turbo intruder, auto repeater, logger++.***
<br>

 - with which type of program a beginner should start hunting and what tip you will give to a beginner who feels demotivated sometimes?

   - ***This is a really tough question because everyone has different backgrounds, but if you're looking to find your first few bugs in web applications I'd check anything with a large scope and low/no payouts. Bonus points if the org has different stacks/tech at play.***

   - ***If eligible, I'd check out https://hackerone.com/deptofdefense. The scope is absolutely massive and the systems in use are managed by different people who use different technologies. Pick a few subdomains that look interesting and use a methodology to try to find some bugs.***

<br>

 - Do you ever take notes while hunting, and if you do, how you structure them? If you dont take notes, how do yoy manage all of the information you have found out about a target?

   - ***Yup, but they really don't have any structure. I use notepad++ and throw a bunch of text in for things that are interesting to me. I've been recently keeping Burp Suite project files and going back to them when I stumble upon interesting stuff.***

<br>

 - how long have you been doing BBs? Are you doing it full time? You Also have a day job? Where do you get your inspirations for new bugs from? Do you hunt only certain bugs? If yes, roughly how many bugs do you look for? 

    - ***I've been doing bug bounty for about 3 years on-and-off and do not currently have a day job. I find a lot of inspiration from the community and try to stand on the shoulders of those doing awesome research. I do not really restrict/focus on particular vuln classes.***

<br>

 - Who should I be following in the appsec/bb world?

   - ***I'd suggest having a healthy mix of everyone involved within vulnerabilities. Follow a few developers, hackers, lawyers, cryptographers, and everyone who contributes to security and bug bounty existing. For research specifically, there are way too many to list! :)***

<br>

 - Your checklist for testing webapp ?

   - ***Don't really have one. I'll generally follow [@jobertabma's](https://twitter.com/jobertabma) advice of***
     1. ***exploring the web app as a normal user would and understanding how it works, then***
     2. ***checking the behaviors you've learned through the normal usage. Cheers.***

<br>

 - Which tools you use And what is your methodology to approach IDOR/SSRF/RCE/CSRF

   - ***Just Burp Suite :)***

<br>

 - As a beginner, I was unable to find those hidden gems earlier but it never been so late 
 1. Is it worth to path traversal a particular target if it had any firewalls? if yes then please give some tips
 2. what tools you use other than burp and do you use any automation tools?

    1. ***Yes, you'll often find simple bypasses like .%2e/, ..;/, and .././***
    2. ***Not many, really. Just scripts I've built myself or intruder. I really enjoy manually hacking.***


<br>

 - Any tips on Subdomain Takeover?? I've been trying to learn this these days. Trying it on VDPs. I also tried automated tools. Did not find any.


   - ***These are really tough for active programs since they're often fully automatable. Your best chance (if you're not trying to automate everything) is paying attention to the error messages for lesser-known services which indicate the service is "unclaimed" or similar.***


<br>

 - Many BBPs have Github included in their scopes. How to test it to earn bounties? Do I have to learn source code review for it or something else? Kindly provide a guideline. Thank you.

   - ***Learning how to query for secrets, credentials, or accidentally committed source code can get pretty complicated but the key idea is just exploring repositories managed by employees. No, re: source code unless the program is open source. If sensitive code is exposed, report it.***

<br>

 - I am learning about #bugbounty since a while. I think I learned the essential but I am unable to do recon very well. I sometimes leave by discourage. How to do in this case?

    - ***Recon really isn't super necessary unless you want it to be. If you have a process you enjoy following or functionalities you enjoy testing I'd really embrace that and specialize in something interesting to you.***

    - ***Lots of bugs aren't the result of "processes" and are combinations of understanding where you innovate or do something creative at the end. If you embrace this and develop a methodology specific to yourself, I think hacking will be more fun to you and come naturally.***

<br>

 -  what was your first bug on hunting platform & was it rewarded? If yes then what was your first bounty & what are the key practices you did to become who u are ??

    - ***My first bug that wasn't rewarded was a pretty lame duplicate XSS. Just a lot of hacking random stuff. :)***

<br>

 - Any suggestions that you would like to give yourself earlier ?
   - ***Mostly just understanding how the program operates from the other side of things. I used to naively think that what I was submitting was the most important thing they saw that day, but looking back, it most definitely wasn't. Triage is hard. Programs are hard to run.***

<br>

 - When did you started your bb journey or cybersec? How do you watch yourself in next 5 years? Whom did you admire while starting back? How do you maintain your mental health? Your favourite movie? Good luck ahead mate! Hope to see you in near future!😉❤

   - ***I've been doing bug bounty since around ~2017. In the next few years, if I am still doing bug bounty, I hope to collaborate with more people and do more development. For mental health I try to pay attention to when I need breaks. Favorite movie is Almost Famous! Cheers***

<br>

 - As the leading expert in path traversals, how many paths have you traversed in total?

   - ***after searching all of my Burp Project files the answer is somewhere around ~ 600.***

<br>

 -  first of all, your blogs are awesome. As a beginner, I was unable to find those hidden gems earlier but it never been so late 
    1. Is it worth to path traversal a particular target if it had any firewalls? if yes then please give some tips

    2. what tools you use other than burp and do you use any automation tools?

   - ***Hey! Thanks for reading, it means a lot :)***

     1. ***Yes, you'll often find simple bypasses like .%2e/, ..;/, and .././***
     2. ***Not many, really. Just scripts I've built myself or intruder. I really enjoy manually hacking.***


<br>

 - First of all your blog posts are amazing.
I really enjoyed and took one where you wrote " Don't force yourself to become a bughunter".

   1. What would be your advice for beginners? Should I master one bug and move to other or look at different types.
   2. What is your favourite bug?

      - ***Hey! Cheers! Bug classes are fantastic for gaining an initial understanding of web security, but to scope yourself to a few where you master them can make you lose sight of the actual process of finding vulnerabilities. I'd use them as tools with the goal to find impactful issues***

      - ***If you pick something like XSS and make it the only thing you care about you can really go about understanding it (which is great) but you shouldn't have your goal as "mastering" a bug class, more so always being "how do I find something the program will care about?"***

<br>

 - I'm curious to know that do you plan on getting a job at some point or do you just prefer doing bb's fulltime? I'd like to understand if you conduct any recon or automate your content discovery for wildcard scoped domains, or are you mainly hunting on main web-apps that has lots of features to play with? It's a question of whether you enjoy finding obscure hosts vs bugs on main webapps.
   
   - ***I prefer hacking on things that have a lot of functionality/different components. I think I'd be uncomfortable relying on recon for the majority of my work but like to be organized/have good information about what I'm attacking so I use a panel that saves metadata.***

<br>

 - Sometimes I pick a program , start testing it, get multiple red flags and then I just don't have motivation to test it anymore...
Maybe cos of my inability to make the most of these red flags and u can take weeks before forcing myself to keep testing them and then I might just switch to another program...this is how it has been for a while .has there been any of your bugs you got by forcing yourself to hack something you didn't wanna?
Or do you think I need to discipline myself or follow instincts

   - ***It's tough. I have a weird relationship with discipline as I did not learn that way. I'd suggest making hacking something you can enjoy versus "enduring" it. It'll be easy to convince yourself "hacking sucks" after a week or so of forced learning. Find community/make it fun.***

<br>

- Whats your interesting findings yet? Where you will see in the 5 years? Any goal?

  - ***I have a few things that I've blogged about @ https://samcurry.net/ and plan to blog about moving forward. Have found a few neat zero days and CVEs that I hope to be able to talk about soon. No real 5 year goals. Just want to be doing interesting and helpful work.***
  
<br>
  
- we come to a situation which is kind of deadlock and we are stuck at one place. We cannot find any interesting bugs. What do you suggest to cope up with this?

  - ***Hard situation. In my experience, while under time constraints, I can never focus on anything. I've fixed this by trying to forget about the situation and just pay attention to what I'm hacking. Once you get one good bug (the hard part) they seem to flow easier.***
  
<br>

 - I'd love to hear more about the psychological side of things when it comes to your experience with full-time bb hunting. Because I think it's as important as the technical. What are the constant challenges you might have faced and how you were able to overcome some of these?

   - ***It's really tough sometimes. At this point I've pretty much identified what are probably unhealthy burnout cycles. My schedule is pretty open so I'll do maybe 2 weeks not doing _anything_, then hack for a week ~60-70 hours. I'm trying to move towards a more regulated approach, but it's honestly been hard to muster the same energy in a normal routine. All of my cool bugs seem to be found manically at like 2-3 in the morning and it's really hard to replicate that within a normal schedule. Some of the challenges I've overcome seem to be very simple issues, but for me were incredibly challenging. One of the main ones for full time bug bounty was following a routine for simple stuff in my every day life. I was able to make myself study chess (kind of silly, but fun) nearly every day for the last year.***

   - ***I'll struggle with the cliché issues like not getting paid for a few months or taking risks with new programs, but I really haven't had too many bad experiences with these. Mental health issues get rough in the winter but I try to exercise when it gets rough.***

     - 

<br>

 - Where did you get interest in bug hunting?
Your first bug? And fav bugs that you hunt?

   - ***I'd been hacking video games for a few years before I found bug bounty. I've always been naturally curious with computers and enjoyed figuring out ways to beat systems. My first bug was a pretty lame XSS. My favorite bug class right now is directory traversal.***

<br>

 - what's your recon flow for oath Inc subdomain finding amass unique script or anything else out there.

   - ***I'll typically find one or two apps which look interesting from a screenshot set using a tool I threw together and dig deep on them. APIs and custom applications are always super interesting to me on Oath.***

     - any suggestions on how to dig deep beyond you know the tip of 100k subdomains that are useless that should of been my question lol

       - ***It's really tough: a lot of what you see in bug bounty is lots of experience identifying weird behaviors. To catalog everything which could be used to "notice" if one site is more vulnerable than the other would be nearly impossible. You'll learn with experience, mainly. :)***

<br>
  
- There are so many cases we should test in an Web App. How do you make sure that you are testing each of these cases?

  - ***To be honest, the only limitation here is time. You're never going to get to test everything, everywhere, and if you do then it'll become too confusing too fast. The trick people use to find bugs is understanding what bugs to test for and where. People who hack on Facebook will tell you that it's often not worth the time to test for standard bugs (XSS, SQLi, etc.) because they've built their system in a way where it's much harder. They instead look for logic bugs and access control issues that seem to be much more common***

<br>

- Hey what do you think about ctf's , does it helps in bugbounty
  
  - ***Hey Yash. CTFs are great. Lots of very smart people and a great community. They may not technically represent real world vulnerabilities, but they're great at introducing people to issues and problem solving. Would absolutely suggest it.***
  
<br>

 - I finished reading "the book" a few weeks ago. Doing portswigger labs and web CTFs. The number of things and ways which we may inject into a real web app is an insanely huge number. This freezes me a bit. Technical and pschological aproaches for making sense of a app?

   - ***I've found that setting small goals for findings can sometimes give you purpose to look for particular issues all the while continuing to test for various other things. If you set a goal of "I want to takeover a user account", it becomes much easier to look and explore logic that relates to that class of vulnerability, all the while passively sitting and watching all of the traffic where you'll probably notice things which indicate other vulnerability classes.***

   - ***I don't think anyone hacks where they actively analyze each parameter for each vulnerability class (and if they do, they're probably overwhelmed) but more so tries to pay attention as things go by and then narrows their focus to certain issues based on their understanding.***

<br>
  
- what would you do after you have found 70-80 subdomains? Will you do dirsearch for all the subdomains one by one or you at all don't do recon that much? Thanks in advance. 🤗

  - ***If it doesn't rate limit or ban me, then everything.***

<br>

 - What type of vuln you look into the programs which are very old where low fruits won't work or csrf,idor all thesetype won't work. Programs like paypal?

   - ***Hey! For these programs I'll look for hidden functionality or things that aren't easy to access (e.g. with PayPal I'd check out programs you have to apply for, management applications, etc.) then go as hard as I can at them. Explore interesting logic and ignore easy issues.***

<br>

 - How & what's your approach to test for server side vulnerabilities ? is it putting paylods for each parameter and expect an interesting response or cves scanning or ... etc ? and thanks in advanse
    
   - ***Mostly always manually checking for them. Most of the server side vulnerabilities I find now a days are in APIs. I'll see interesting behaviors (e.g. /api/fetchUser) and play with it (read docs, guess params, etc.) until I understand that it's _not_ vulnerable.***

<br>

 - how i could be better in Path traversal like you? I see you are very good at this! 😍i don't know when i should looking and digging for path traversal. How do you know when you should digging more into it? When we should fuzzing? Thank you very much!! 🤪


   - ***When I hack with others they'll often tell me that I spend too much time on things that are likely not exploitable/end up being unexploitable. This is often a waste of time, but I think has let me understand how to tell if something is worth exploring more. I'd try to play around as much as possible with URI behavior and anything that even slightly looks like a path parameter (?id=/foldername/file) and understand what errors are simply bad request/false positive and what requests indicate you're within a secondary context. Cheers.***

<br>

 - How do you treat a potential bug when you don't know much about it to test further? Ask someone till you get it or Just move on to looking for another one
   
    - ***These are always interesting cases, but I'll make note of it and try to grab inspiration/understanding by exploring similar functionalities. There was a bug recently where an API took JSON in an unknown format. I explored the rest of the app and found the format eventually.***

    - ***Rabbit holes are always exciting but knowing where to stop is hard. With more time hacking it's easier to tell, but I don't believe there's an objective end to every endpoint. There will always be new techniques. Keep stuff on a backburner.***

<br>

 - Some people are wide-and-crazy recon people while some just test core functionality ...
In a case where I have limited mobile data and power supply, what would you suggest? AND What's a good next place to look after directory brute force with no bug?

   - ***The first approach that comes to mind when testing with low power and limited mobile data is phwd's approach. They seem to do a lot of JavaScript analysis and do most of their testing within their browser. Check out https://philippeharewood.com if you haven't already.***

<br>

 -  you are good at understanding bug from weird behaviour on response. How do you know it when to continue or stop to test a request. Is it knowing the tech are important to understanding how the directory routes is?

    - ***Thanks -- I think knowing the tech is important but not necessary. If you notice it's apache and observe a 400 bad request with GET /../, it's pretty clear what's going on, whereas if GET /../ returns a blank 200 and you don't understand it's probably worth more time.***

    - ***There are a _lot_ of false positives with directory traversal but understanding proxy functionality or system API calls which reference files makes it a lot easier to know when to give up and move on. I'd recommend exploring some proxy write ups, will share some soon here [@samwcyo](https://twitter.com/samwcyo)***

<br>

 - besides screenshotting, do you have any tips on finding interesting places to look at on large scope targets?

   - ***I think that each asset is super different but irregularities and understanding patterns will help with identifying things to poke at. An example would be a JSP site where everything else is PHP, different APIs with weird prefixes (e.g. dev-api), things like that.***

<br>

 -  what do think about codeQL ?

    - ***It's a super cool approach to finding bugs. I really love the idea that Github understands the ways in which they can leverage their platform to eliminate security vulnerabilities. Really enjoyed findings by people like [@JLLeitschuh](https://twitter.com/JLLeitschuh)
 exploring this approach.***

<br>

 - Do you know about zeodium? If yes please give some info about it.

   - ***Hey Yanda. I've looked into Zerodium a lot but have never used it. They'll purchase vulnerabilities affecting common products/softwares and post bulletins for what they're looking for. It's unknown what they'll use your vulnerability for but it's someone who can afford the price.***


<br>

 - Do you use any paid service related to Bug Bounty/Security? If any, then how much? and also do you refer any to others

   - ***I'm paying $5/mo for a Digital Ocean box which I use for various scripting and directory brute forcing. Besides that, nothing really. If I were to use anything that was paid for it'd probably be a recon service where it's a management dashboard style app.***


<br>

 - Fuzzing and fuzzing automation. 😃

   - ***Fuzzing is great, but I am not so great at fuzzing automation. I'd learn how apps respond by manually fuzzing different sorts of apps. You'll learn to notice certain error messages (e.g. dangerous control character in Tomcat) and what to try. Throw stuff in repeater very often.***

<br>

 - I want to learn about API pentesting and fuzzing. Can you tell me where should I start? And can you share some bugs you found just by fuzzing the API requests? Thanks in advance :)

   - ***If you already have a bit of normal web app experience then testing APIs should be fun for you. Understanding different API gadgets like swagger and WADL files helps in exploring them, but APIs are basically just huge clusters of functionality...
    Some vulnerabilities I've found fuzzing APIs include silly things like ATO via parameter pollution (id=1&id=2), directory traversal issues, IDORs and a lot of permission issues, and SSRF.***
   
<br>

 - What are the next things you want to focus on or research?


   - ***I've been working on a large project with a few other hackers for the last 3 months and (when it's hopefully finished here soon) can spend some time auditing common software like Tableau/similar apps. I've never really hacked industry apps and have really wanted to. Since the live hacking events have all been cancelled because of COVID we decided to pick a single target and see how many bugs we could find within a two month period. We ended up finding a bunch of neat issues and are publishing a sort of portfolio of the findings. Portfolio as in collection of summaries/deep dives for the particular issues we've found***

<br>

 - what kind of issue will you go for if the scope is too small like only http://app.target.com is in scope and website functionalities to go for, what kind of a strategy or bug type you surely go after?

   - ***It depends on what services the app provides. If there is authentication, then there are a whole sub-classes of things to go after like access control and client-side issues. If the service is very limited without authentication (e.g. blog), then cache deception type issues.***

<br>

 - Which Burp Suite plugins do you use and which one u think is the most important in ur workflow ? 

   - ***I like using JSON beautifier. Kind of boring, but I work with random JSON APIs so much it helps a lot.***

<br>

 - If you could split up your bugs by core application bugs vs recon induced bugs, what would the percentages look like? An estimate is fine.

    - ***It'd be about 85% limited/no recon (subdomain enumeration using Sublist3r or similar) and 15% recon. The pure recon bugs I've found have been very lucky and not super reliable (being the first one to find a subdomain).***
     
      - This is great. Thanks for answering. I would say for me, due to rapid micro site development on targets like Uber, 80% are possible due to recon. But I actually split recon up into depth and breadth. Uber requires both. Finding the asset + reversing the JavaScript.

        - ***It's really interesting trying to put "recon" in a category. I've found tons of endpoints via exploring JavaScript, but I am unsure if the bug would qualify as a full recon bug when the core issue is fuzzing the API call/identifying behavior. Thanks for sharing!***

<br>

 - Hey sam, thanks for doing this! I love reading your posts as you find some really interesting finds, especially this one: https://samcurry.net/abusing-http-path-normalization-and-cache-poisoning-to-steal-rocket-league-accounts/
Do you follow any type of flow when hunting for vulnerabilities?

   - ***for this bug particularly I started hunting for more esoteric issues due to the limited scope. There were only a few endpoints and not that much functionality, so I picked a few places that were points of compromise (authentication) and tried to scrape stuff together.***
      
      - I will follow up to his question if you may, as there were only few endpoints and not much functionality, how do you know when to put a stop sign when you dont find anything at the endpoints? in order to avoid going into a rabbit hole. Thanks!
         
         - ***One of the first things I noticed was that there really wasn't much of an integration with your rocket league game account and the website. There may have been some APIs deeper, but I couldn't seem to find much available or documented. Subdomain enum, Google dork, and browsing.***
