---
layout: post
title:  "Infosec Bugbounty AMA with Sam Curry"
categories: infosec-bugbounty-ama
---
# AMA with [Sam Curry](https://twitter.com/samwcyo)

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

- while learning about bugs what mistakes you made and what methodology you suggest to learn a bug ? Did Recon is neccessary to learn especially for beginners..? what is methodology while a hunting bugs..?

   - ***I made the mistake initially of depending on other people for things I could've learned myself and ended up digging myself into a hole when I went back to figure it out. Recon is not necessary but if you enjoy it then go for it. See other replies re: methodology :)***

<br>

 - What kind of vulnerabilities do you like to go for first?

   - ***Nothing in particular, to be honest. Just keep my eyes open for whatever fits the situation.***

<br>

 - what suggestion you give for beginners from your mistakes

   - ***When I first started bug bounty I'd sent a few dozen PMs and nobody had responded to me. I thought this was a bad thing, but I went out and studied things by myself and learned how to do the majority of work myself. I'd recommend not offloading the core learning.***


<br>

 - Your checklist for testing webapp ?

   - ***Don't really have one. I'll generally follow 's advice of***
     1. ***exploring the web app as a normal user would and understanding how it works, then***
     2. ***checking the behaviors you've learned through the normal usage. Cheers.***

<br>

 - Which tools you use And what is your methodology to approach IDOR/SSRF/RCE/CSRF

   - ***Just Burp Suite :)***

<br>

 - As a beginner, I was unable to fond those hidden gems earlier but it never been so late 
 1. Is it worth to path traversal a particular target if it had any firewalls? if yes then please give some tips
 2. what tools you use other than burp and do you use any automation tools?

    - ***Hey! Thanks for reading, it means a lot :) 1. Yes, you'll often find simple bypasses like .%2e/, ..;/, and .././ 2. Not many, really. Just scripts I've built myself or intruder. I really enjoy manually hacking.***


<br>
 - Any tips on Subdomain Takeover?? I've been trying to learn this these days. Trying it on VDPs. I also tried automated tools. Did not find any.


   - ***These are really tough for active programs since they're often fully automatable. Your best chance (if you're not trying to automate everything) is paying attention to the error messages for lesser-known services which indicate the service is "unclaimed" or similar.***


<br>

 - Many BBPs have Github included in their scopes. How to test it to earn bounties? Do I have to learn source code review for it or something else? Kindly provide a guideline. Thank you.

   - ***Learning how to query for secrets, credentials, or accidentally committed source code can get pretty complicated but the key idea is just exploring repositories managed by employees. No, re: source code unless the program is open source. If sensitive code is exposed, report it.***

<br>

 - Any suggestions that you would like to give yourself earlier ?
   - ***Mostly just understanding how the program operates from the other side of things. I used to naively think that what I was submitting was the most important thing they saw that day, but looking back, it most definitely wasn't. Triage is hard. Programs are hard to run.***

<br>

- Whats your interesting findings yet? Where you will see in the 5 years? Any goal?

  - ***I have a few things that I've blogged about @ https://samcurry.net/ and plan to blog about moving forward. Have found a few neat zero days and CVEs that I hope to be able to talk about soon. No real 5 year goals. Just want to be doing interesting and helpful work.***
  
<br>
  
- we come to a situation which is kind of deadlock and we are stuck at one place. We cannot find any interesting bugs. What do you suggest to cope up with this?

  - ***Hard situation. In my experience, while under time constraints, I can never focus on anything. I've fixed this by trying to forget about the situation and just pay attention to what I'm hacking. Once you get one good bug (the hard part) they seem to flow easier.***
  
<br>
  
- There are so many cases we should test in an Web App. How do you make sure that you are testing each of these cases?

  - ***To be honest, the only limitation here is time. You're never going to get to test everything, everywhere, and if you do then it'll become too confusing too fast. The trick people use to find bugs is understanding what bugs to test for and where. People who hack on Facebook will tell you that it's often not worth the time to test for standard bugs (XSS, SQLi, etc.) because they've built their system in a way where it's much harder. They instead look for logic bugs and access control issues that seem to be much more common***

<br>

- Hey what do you think about ctf's , does it helps in bugbounty
  
  - ***Hey Yash. CTFs are great. Lots of very smart people and a great community. They may not technically represent real world vulnerabilities, but they're great at introducing people to issues and problem solving. Would absolutely suggest it.***
  
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

