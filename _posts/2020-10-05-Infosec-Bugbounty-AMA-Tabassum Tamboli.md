---
layout: post
title:  "Infosec Bugbounty AMA with Tabassum Tamboli"
categories: infosec-bugbounty-ama
---
# AMA with [Tabassum Tamboli](https://twitter.com/Tabnexa)

<br>

 - How much time did it take to find ur first bug what was it and any stater tips for beginners

   -***In early phase I found many bugs on non rdp sites. 1st paid bug worth 100$ after 10 months. Don’t go for dollars, Try to learn command line and understand tools how they work. Then go for understanding application.***

<br>

 - What was your motivation to take this    path? Did face any backlash from the society?
    First bug you found?
    Small advice for beginners in webapp hacking!

   - ***3 years ago I started application testing because of Aditya. We both graduated from same college. Yes I faced many bumps from society to downgrade my profile but I never give up. Frankly speaking my first bug was clickjacking 3 steps on delete account***

<br>

 - What should I do when I get mentally drained by N/A & Duplicate & what was the most toughest & challenging bug you ever found ??

   - ***NA and dups are very frustrating, idk how people handle it.  I used listen songs and drawing pictures.*** 

    - ***Challenging bug: IDOR to delete account, That time I was not able to get uuid.***

<br>

 - your favourite bugs , how you learn about new vuln types

   - ***Favourite bug: CSRF. I used to google it at first phase and then I check for types of vulnerability and reports related to it via h1***

<br>

 - What's the interesting bug you found while hunting? 
And any weird bug which you paid for it?

   - ***I was able to see tickets and bugs reported by other hackers and I totally gave this credit to my friend [@ADITYASHENDE17](https://twitter.com/ADITYASHENDE17)
 for teaching me.***

<br>

 - at what age u started your bugbounty journey?

   - ***3 years ago....***

<br>

 - What was the most difficult phase while getting into cybersec

   - ***People used to show no respect to not only me but also for other girls too in infosec community. They still think all girls used stop scooty using legs
   Face with tears of joy
   .I don’t care about it. I love what I do.***

<br>

 - you use automation for your recon and other stuff or just manually do it?
your favourite recon tools?
How many dupes you got before your first valid bug submission?
Your favourite book till now for cybersec. ?
which type of bug you look first i mean which bug you love to find?

   - ***I don’t use automation on high level. Tools already posted on another tweet. I didn’t count for dup, but I got bounty after 10 months . I love to find CSRF***

<br>

 - I'm about to graduate college. Just one sem remaining. I'd love to take up an infosec role right after college. But my parents are not so supportive quoting that infosec doesn't pay noobs like me well. Do you recommend I take it up right after college?

    - ***Don’t give up. I started from nothing . I used have very less money in pocket. For testing purposes I was using public wifi to save quota of net. Convince your parents wisely.***

      - What are my options if I go for it? Does companies take in noobs like me?

        - ***Without skills and hands on experience they will reject your application. So it’ll be better if you start on skill wise***

<br>

 - I'm a final year cs student and want a job in infosec, so should i put my hackerone profile in my resume & where to find fresher's infosec jobs in India?

   - ***Yes. You can put your profile for reference. LinkedIn platform will help you get job n more reach. There are many job portals where you can apply or else you can go via reference of your friend who is working in company.***

<br>

 - What is your priority to your bugs? 
Quality or Quantity ?
Means you wanna find more bugs or Wanna find 1 good bug 

   - ***I want to find more bugs.***

<br>

 - Your Recon tips :)

   - ***Currently using assetfinder, httprobe for basics.***
   - ***Github recon learned from gentleman.***
   - ***Checking js files for sensitive information Wfuzz, ffuf and dirsearch alot.***

<br>

 - Any tip for 2FA bypasses ?

    - ***Cve based: Checking version in responses. Googling for known exploit also github to search more information.*** 

    - ***Now nuclei for extra power***😅 

    - ***For otp: Tampering response. Brute force otp, Passing null values in otp section, removing parameters***

<br>

 - How I found my first CSRF ? Tips please 😊

    - ***Checking all functions even if there is token you can bypass it with various method. I usually perform csrf attacks on account update section***

<br>

 - Are you using custom wordlist or using wordlist from seclist

   - ***Seclist and brute force list of random robbie***

<br>

 - How i find information disclosure bug /sensitive data plzz guide me ?

    - ***Dirsearch, Google Dorking, Github Dorking , Source code analysis, Js files checking, Sending crash payloads to get weird response.
    Etc***

<br>

 - Picking a vulnerablity and trying to hunt  on many different web apps, or understanding one webapp completely and hunting for logical bugs or according to functionality given, what do you prefer?

   - ***According to functions you can abuse it. So it’ll be better in my view.***

<br>

 - What is your recon methodology...?
    How you deal with burnouts..?
    Fav bug and any tips for LFI

    - ***Grabbing subs . ASN , Cidr ranges . Lookups for services. #
    Sorting live subs > fuzz all with ffuf in one time. Checking for login pages and signup too. Wayback for URLs. Js file analysis. Github recon and subjack for sto.***

<br>

 - Do you have or plan on taking any offensive security certifications? Are you bug hunting for a long time now? How much do you enjoy this? How many hours per day do you hunt? I'll stop now cause I have already asked a lot of questions😅

    - ***Not that much experience for oscp now, but surely in future I’ll grab oscp cert. Doing BB from last 3 years . Per day I used to spend 4 hours , in morning 2 hours and night for remaining testing***

<br>

 - How do you test for cve based bugs and any tip for otp bypasses ??

    - ***Cve based: Checking version in responses. Googling for known exploit also github to search more information.*** 

    - ***Now [nuclei](https://nuclei.projectdiscovery.io/) for extra power***😅 

    - ***For otp: Tampering response. Brute force otp, Passing null values in otp section, removing parameters***

<br>

 - Ffuf or Dirsearch?

   - ***1st priority for Ffuf*** 

<br>

 - Which is the inevitable tool u use in ur workflow ? 
Do u use any unique tool that others don't use frequently ?

   - ***I do use same tool which other people have. Waiting for correct time is key for data***

<br>

 - What was your approach for small scope ..?

   - ***Approach is same for all but if domain have less scope then I fuzz alot and everything***

<br>

 - Any resources to learn more about ATO?
if a target have a firewall which bugs are worth finding according to you?

   - ***For finding ATO you can go with medium write ups and mostly idors on sensitive actions which related to account functions.***
     - ***Auth issues*** 
     - ***Csrf***
     - ***Idor***
     - ***Host header on reset function*** 
     - ***Password abusing***

<br>

 - how to deep dive into a ecommerce target any tips? and also any tips on targeting an  authentication mechanism

   - ***For e-commerce sites make sure you are able to bypass or abuse payment gateways, this are high paid bugs.***

   - ***Example: While payment they’ll ask for otp so instead of that you can directly manage to use default URL to bypass otp while payment. Price manipulation also***

<br>

 - How do you test for email related features ? Like during sign-ups or when inviting someone via email and stuff

   - ***Adding multiple id in request and checking for all mails to verify link is same or not. Registering acc with company mail addresses for extra privileges m. Checking for oauth redirection while signup to bypass verification . In invites I check for HTML injections***

<br>

 - Any resources for desktop based application pentesting ?

   - ***I love this blog. Hope you’ll like it [NetSPI Blog](https://blog.netspi.com/introduction-to-hacking-thick-clients-part-1-the-gui/)***

<br>

 - any specific methodology for XXEs ?

   - ***If any function fetching data from backend and transmitting in XML parse from browser to server you can test for it.***

    - ***Request body exploitation is better to understand and observe it. Or else try to change content type. I got xxe for 3 times only. So that’s what I know.***

<br>

 - 

   - ******