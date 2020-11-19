---
layout: post
title:  "Infosec Bugbounty  AMA with Sreeram KL"
categories: infosec-bugbounty-ama
excerpt: " AMA with Sreeram KL "
author: Ravi Shankar Gurram
---

# AMA  with [Sreeram KL](https://twitter.com/kl_sree)

<br>

## Bug Bounty hunter ,💥 top #50 at GoogleVRP 💥

<br>

 - How much time it took for you to find the first bug from the time you started hacking?

   - ***It took around 8 months for my first valid bug. (Started with 0 knowledge on programming or how computer works)***

<br>

 - How did you learn bug bounty hunting? And how do you practice your skills and keep yourself up-to-date?

   - ***Write-ups, talks and CTF are the best way to learn bug hunting/security. CTF helps a lot in practicing to detect and exploit a vulnerability. [@PentesterLand](https://twitter.com/PentesterLand) have an awesome list of bug bounty writeup, check that out!***

<br>

 - which language do u prefer for me (beginners) for bughunting...what is yur first server side bug..what motivates yu when u get duplicate.

   - ***I recommend you to learn javascript, it can help you both in front end and backend. By learning something that's heavily used, you can easily spot vulnerablites in it. My first server side bug was admin panel bypass (blank credentials***😅😅 ***).***

   - ***I force myself to hunt different classes of bugs, so even if I get duplicate I'll learn something new.***

<br>

 - What are your favourite vulnerabilities to look for, when starting on target?

   - ***I love client side vulnerabilities. While hunting I test for almost all client side vulnerabilities & SSRF.***

<br>

 - Do you take notes while hunting if yes can you explain in briefly

   - ***I don't have an organised note. But whenever I find an interesting endpoint or an idea pops up I note it down. It's comes really handy . I use http://hackmd.io***

<br>

 - How do you choose a target while hunting on google. Do you hunt Google's main domain or acquisitions?

   - ***I choose target I'm familiar with and the one I use regularly. I prefer main domain over acquisition, cause it pays around 30x more (incase case of xss)***

<br>

 - How you start at GoogleVrp. Recon for Google. Tips for Google.

   - ***I prefer to go with the applications that I'm already comfortable with . I just do subdomain enumeration while hunting on Google. Google does not use third party products extensively, they build (protobuf),so get familiar with the technologies  before testing.***

<br>

 - How do you do recon? Do you have any kind of notification system for code pushes , updates and new assets ?

   - ***I'm not a recon guy. I prefer hunting in main apps. In past I tried building some notification system for asset update. It worked and got some bounties,yet lazy to have it.***

<br>

 - How do you approach finding bugs in Google

   - ***I look for similar bug classes that are already documented in writeup by people bug hunting on Google.***
     
     - where do u get that writeups?
        
        - ***Twitter and [@PentesterLand](https://twitter.com/PentesterLand)***

<br>

 - What kind of recon methodology you use while hunting on small large and medium scope targets

   - ***In case of recon the most I do are Spidering endpoints, waybackurls, subdomain enumeration and github for credential leaks. If the scope is very small, fuzz everything possible! You end up finding something.***

<br>

 - For learning xss, do you think a person should have a sound knowledge in JavaScripts. Do the basic xss payloads works these days?

   - ***I started learning xss with zero knowledge on JavaScript and it worked for me. Having a sound knowledge in Javascript will help you a lot. I recently found some severe vulnerabilities solely through javascript (not xss) . Basic payloads still seems to work(alteast to me).***

<br>

 - Is Bug Bounty lucrative enough to be self employed?

   - ***Not really (to me), there  were times when  I get no bugs for straight 3 to 4 months. If you're curious try it and see how it works for you.***

<br>

 - When I come across 404 pages and check the cname they were pointing to some other things which were not there in ed overflow github and also on hackerone reports. Any suggestions for this?

   - ***Subdomain takeover can only occur when the cname it's pointing  can be registered by the public. Check if you can register that domain.***

<br>

 - Have u faced locked out of your own accounts while hacking on google

   - ***Not yet.***

<br>

 - Tips or your methodology on approaching Http Desync attacks and SSRF, Open redirects. Also, why you are well known as satellite boy :D

   - ***I haven't found a HTTP desync attack in real world application, so can't give a tip on that. SSRF, test ssrf attacks through file parsers (pdf, zip, xml) , many miss that. Open redirects, always try to escalate it to xss, ssrf.***

   - ***IIRC I got admin access to YouTube's "Satellite multiplexer " via blank password, and that's the history behind that name!***

<br>

 - What are pre-requisites for Android BB Hunting? for Example: knowledge of Java, etc...

   - ***I'm not really into Android BB, AFAIK you need to get a good understanding of Android security model before starting out,it's pretty different from web.***