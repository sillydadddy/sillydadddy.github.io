---
layout: post
title:  "Infosec Bugbounty  AMA with Mehedi Hasan Remon"
categories: infosec-bugbounty-ama
excerpt : "AMA with Mehedi Hasan Remon"
author: Ravi Shankar Gurram
---

# AMA with [Mehedi Hasan Remon](https://twitter.com/remonsec)

<br>

 - If we ask you to begin again in bug bounties  .what's gonna be your plan ?

   - ***Well, it was a nice question. I would like to learn the basics so deep so in the future I can explore my targets more deeply. In beginning learning basics really so boring and no fun. i scraped some topics and now suffering for that***

<br>

 - For beginners...focusing on one vulnerability and trying it in every website is better? or learning the owasp top 10 and trying it in a single target which one is better approach.

   - ***it actually depends on that specific person. It actually dosent matter. Just learn all the basics. then chooce one topic or area to become master on it. you will get bugs that are not even listed one OWASP top 10 may oneday you discover your very own bug. so why you waiting for***

<br>

 - I am leaning websec from 4 months still not able to achieve anything significant .... any tips?? I know theory... but while testing real target  I couldn't able to find anything !

   - ***Before joining bug-bounty I use to do some kid blackhat stuff. like dumping data with sqli and bypassing file upload protection to get a shell. So that time I was dealing with all real websites. somehow I already had confidence before joining bug-bounty.***

   - ***You can use this idea for your benifit. like first targets websites those dont pay cash or less crowded. then make your hands dirty there. poke them as much as you can. you will get a idea or at least some level of confidence. then you can start hunting on regular bugbounty sites***
  
   - ***But make sure you are going for programs with responsible disclosure policy. Dont just poke every random website. it may be illigal. use google dorks to get some small self hosted program***

<br>

 - Platform you recommend to beginner. Your Most Critical Vulnerability that submitted. Program that you hunted on the most.

   - ***[@Hacker0x01](https://twitter.com/Hacker0x01), [@Bugcrowd](https://twitter.com/Bugcrowd) VDP can be a good way to get started with a platform for beginners. I found 25+ bug in 2 VDP that helps me a lot to boost my confidence***
   
     - ***It was an RCE in http://silvergoldbull.com***
     - ***I hunted most on [@SamsungMobile](https://twitter.com/SamsungMobile) [@SamsungTV](https://twitter.com/SamsungTV) They pay via [@Bugcrowd](https://twitter.com/Bugcrowd)***

<br>

 - How do you manage your time between enjoyment, learning, friends, education, bug Bounties?

   - ***BugBounty is enjoyment itself. When i recieve bounty i use to hangout with friends. Then start leaning and hunting again till i get a new cool finding or cool bounty.***

<br>

 - How to search VDP programs

   - ***Umm, you can go with the platform public VDP list. They may be more crowded so you also can do some google dork to get programs that are invite-only or not visible on the platform. Let me give you one, [@McAfee](https://twitter.com/McAfee) They will invite [@Hacker0x01](https://twitter.com/Hacker0x01) and they really have a huge scope***

<br>

 - I am an eng student who just entered this domain a couple of months ago. I have mastered Linux & some of the tools but my main interest is to make my own using python & AI. Do u have any suggestions? Am I too ambitious or should I stick with a conventional approach.

   - ***while it comes tooling time always keep your mind the tool you use or want to use does it fit your workflow pipeline. or actually you know well why you will use that tool. Coz tool just make the actual work easy for you it will not do the work itself for you***

   - ***In general [@golang](https://twitter.com/golang) tools are more popular in bb community***

<br>

 - When you pick a target, exactly how you start testing it? What are some common vulnerabilities you always look for in your target? 

   - ***There usually 2 way I follow to pick targets***
     1. ***Mass Targets***
     2. ***Single Target***

   - ***Mass Targets***
     - ***Pick one vuln & search them every target***

   - ***Single Target***
     - ***Pick one target search every vuln there***

   - ***Common Vuln***
     - ***Well common vuln only works on mass attack.***

   - ***Like you can search sub tover in all programs but when target is specific it may not work at all. So then understand the target and approach how it designed or works***

<br>

 - do you look for large scope programs or small scopes ? your favorite vuln type ?

   - ***Till now I was looking for large scope programs as I do recon so deep and my fvrt vuln type is Information Disclosure. But I want to push the game further. So now choosing small scope programs and bugs that require more manual effort and a deep level of understanding***

<br>

 - What is your approach for recon? And what are the main tools you use?

   - ***I use a terminal and [@httpie](https://twitter.com/httpie) I follow [@PentesterLand](https://twitter.com/PentesterLand) cheat sheet c posts. It helped me a lot. The scenario is different everytime for different program. So I am not getting the idea how can I explain it to you. But I will release a blog post soon about my recon approach***

<br>

 - When you aproach a target for testing what are the main recon and testings that you do most offen or any common way in process to find bug's.

   - ***For recon follow [@PentesterLand](https://twitter.com/PentesterLand) cheat sheet [@httpie](https://twitter.com/httpie) blog posts. There will be some quick shot approach. But those things will come only based on your experiance. So you get the idea it's hard to explain point by point.***

<br>

 - what is your approach for finding information disclosures, Like for info disclosure how you approach after you select your target?

   - ***Collect as much subdomain as i can***
   - ***Fuzz every subdomain***
   - ***Collect all js and analyze***
   - ***Do mining for fuzzed endpoints***
   - ***Do GitHub Recon***
   - ***Check Webapps on nonstandard ports***
   - ***Now you have a general view about your target***
   - ***Play with all the assets, Game start now***

<br>

 - What’s your approach when finding logical/business flaw bugs? Any specific tools you use for xss?

   - ***For finding business logic bugs first use it as a normal user. If possible take note about all functions and feature. Then abuse those areas, maybe by tampering with values or using it how it not build for. H1 disclosure reports may help to get the scenarios on mind.***

   - ***For xss I found dalfox by [@hahwul](https://twitter.com/hahwul) kxss, waybackurls by [@TomNomNom](https://twitter.com/TomNomNom) useful. But you may not always get quick xss with oneliner. So good to use reflector burp extension to see reflected Params. Also create regex for replacing your keyword with xss payload.***

   - ***Specially dig for hidden Params on login pages or other endpoints. Hidden Params can be a good place to test for those injection attacks***

   - ***I tried my best to show you my full support. Hope you get the idea. If need any more info feel free to ask*** 😃

<br>

 - Tips for XXE and RCE.

   - ***You can follow bugbounty cheatsheet and github repo for those resources. there you will get a lot of things about specific vulnerability classes***

<br>

 - Can you suggest me an article or video which explains how to use tools like ffuf, amass, nuclei etc in the best way possible

    - ***[@codingo_](https://twitter.com/codingo_) [@InsiderPhD](https://twitter.com/InsiderPhD) [@stokfredrik](https://twitter.com/stokfredrik) [@NahamSec](https://twitter.com/NahamSec) [@thehackerish](https://twitter.com/thehackerish) [@theXSSrat](https://twitter.com/theXSSrat) They are doing this part. make sure you have subscribed to them on their youtube channel.***

<br>

 - your methods to hunt for subdomain takeover bugs

   - ***if i be hones i used http://github.com/remonsec/SEF this tool to get all unique subdomains then using general tools for takeover vulns.***

<br>

 - What are the things you look in single domain? Or site with merely 3-5 Subdomains?

   - ***So you are talking about small scope target. For them go for business logics and also try to get hidden params from each endpoint. that will lead you getting quick bugs. But in general. you may not get surface level bugs there. you have to dig deep on their main application***

<br>

 - How do you fuzz directories/api endpoints? And deal with rate limiting?whats your typical methodology when target has small scope?

   - ***If i be honest i dont do fuzz for small scope. Coz there you have to put a lot of manual effort to understand the target first. So its hard to get something from surface level. But nowadays i found mining hidden param on different forms with Arjun working well***

<br>

 - Automation VS Manual workflow %? Top 3 bugs you instantly look for manually? Bugs you only look for w automation?

   - ***Actually it's not like automation vs manual it's like Automation + Manual. Overall it depends on different hunters mindset and skill how they use those ideas. I just do them both. Learning new bug and understanding it well then write some code to give it a automated shape.***

   - ***Top 3 custom bugs I always look for manually***
     - ***Misconfigured endpoints*** 
     - ***Webapps on nonstandard ports*** 
     - ***Improper Access for those misconfigured areas***

   - ***I always make sure that I have enough deep subdomains for getting those bugs. Coz they usually rise for lake of attention***

   - ***When I become good at those specific bugs I design a workflow to find them automatically. Shell scripts do the work for me. Even for subdomain takeover I also check web screenshots. So I don't look for bugs automation only. I do both automate and manual for each bug I know***

<br>

 - do you Advise about any useful tools to get hidden params? and what is top 5 vulns you find it ?💙

   - ***For get hidden param I use Arjun by [@s0md3v](https://twitter.com/s0md3v)***
 
   - ***my top 5 vuln classes is***
    - ***Info Disclosure***
    - ***Subdomain Takeover***
    - ***Business Logics***
    - ***Improper Access Control***
    - ***Content / Html Injection***

<br>

 - Do you prefer making and using seperate wordlist for every different program or you use seclist?

   - ***it's good to have a collection for specific wordlists and endpoints. you can use them later on in different scenarios. but it also time-consuming. So make sure you are doing it regularly and storing those lists in your collection. Seclist also comes with this type of collection***

<br>

 - Your favorite github tools and burp extension list

   - ***I actually do hunt on surface level much. So in general I use terminal and [@httpie](https://twitter.com/httpie) for burp I found reflector and burp bounty helpful***

<br>

 - How much do you rely on burp-suite while you discover any vulnerability ? From 10/

   - ***I use burp as a network interceptor as it build for. After having the idea about target feature and functions I use burp to send different request on those areas. You also can use burp in different way like to do your webapp recon and other stuff. But I just use it to test areas***

     - Do most of the bugs you discovered without a burp suite?  I do not like the burp suite , but some ppl say it is very important:(

       - ***If I be honest I found 90% of my bugs with terminal and curl only. But yes while testing different feature burp is doing it's best. You also can do same without burp but it will make the work easy. Overall we don't depend or relay any tool we just use them for our work. Right ?***

<br>

 - what critical bug types u mostly look in webapp

   - ***Nowadays looking for private webapp access. like things that i should not see or at least not for me.***

<br>

 - Is port scanning important? How do you hunt for Info disclosure?

   - ***Well I found port scanning over custom permuted and 3rd level subdomains real worth. You will get webapp running on nonstandard ports and they are too much buggy. You can takeover those admin roles easily there.For information disclosure generally I try to bypass protected areas***

     - One more, do u fuzz alot? If so, which worldist that u used?

       - ***Yes I full on each and every endpoints. Seclists and assetnote wordlist works well for general touch. For dns Enumeration you can fuzz with all.txt rest of all depend where you actually doing the fuzz***

<br>

 - If you Search about bugs by google dorks or GitHub.. Do you do this manually?

   - ***I do both manual and automation For google Dorking this may help by [@nahmedfaisal](https://twitter.com/nahmedfaisal)  http://dorks.faisalahmed.me***

<br>

 - how do i start subdomin take over?

   - ***Just start it by collecting as much subdomain as u can***

<br>

 - When you open a subdomain for testing, what are things you take into consideration? 

   - ***First of all understand their business purpose. It may help you to get unique and custom bugs. Then do your recon and test for vuln different functions***

     - How do you work with burp when doing the above task?

       - ***the usages of burp actually depend on what you are testing and where you are testing.***

<br>

 - 😅 How do you test an application that is a part of the Atlassian Marketplace Bounty Program

   - ***I didn't try with Atlassian marketplace programs bro. But I saw people are doing good there. [@pdnuclei](https://twitter.com/pdnuclei) may help you at that point***

<br>

- a question about BAC so for example if user 1 can change user 2 account to private or public by changing user 1 authorization header to user 2 authorization header. is it a valid BAC or bug?
   
   - ***Here the question is how user 1 will get user 1auth header value. But I saw some program accept it and some may not. But in general it will end up with informative or n/a.***

<br>

 - Have you ever though about doing part-time pentest ? If yes, did you enjoyed this experience? I have some opportunities for doing that but I'm quite scared of it 😅

   - ***It will be so awesome. As pentest is actually different form BugBounty. Pentest is easy for bughunters. Coz we already dealing with full blind testing. Do your pentest work and enjoy it. Don't worry it will be easy for you.***

<br>

 - If you find a cve on a website which don't have a bug bounty program will you report it? If yes how will you tell them about yourself?

   - ***If you get something like that then just report it as a general user not like a regular bug hunter. Show that you are helping them by telling about it. If they feel comfortable then take step further and support them untill they fix the issue. How they will reward u as well***

<br>

 - Where are you investing your bounties? :) :D

   - ***Didn't Invested yet. Just brought things that I need and tried to support my family as much I can.***

<br>

- How you overcome Demote and Fails? Do u follow a Checklist?

   - ***Hehehe, Most painful part my brother. Nowadays I no more feel demote or fails. Coz I am already passing an extreme level of this. I just have to keep doing what I like and have to be the best at it. I don't follow a checklist. But yes there always some general workflow***

<br>

 - how many types of bug in jwt(json web token)
Way to bypass

   - ***I don't know about it. But let me mention some who may knows [@hunter0x7](https://twitter.com/hunter0x7) [@ADITYASHENDE17](https://twitter.com/ADITYASHENDE17) [@ElMrhassel](https://twitter.com/ElMrhassel) [@alicanact60](https://twitter.com/alicanact60) [@naglinagli](https://twitter.com/naglinagli)***

   - ***@hunter0x7 : Learn all the methods from [Pentesterlab](https://pentesterlab.com/)***

<br>

 - I remember i got a dupes with you so i wanted to ask how often you hunt on vdp and can you name some sub takeover on non-common services you have found Thank you bro

   - ***Yes dude I also can remember. I use to hunt those programs as experimental hunt. Like doing some new or crazy thing with the knowledge I have. You got a sub tover dup with me. That month I use to perform deep subdomain Enumeration and takeover automation.***

   - ***The tool I used for subdomain Enumeration is now public https://github.com/remonsec/SEF***

     - Bro your tool is osm but using it is a bit difficult as it take a bit longer time and  i get a lot of subdomain but only few of them work so i have to resolve it on my own so can you please add tool to filter only live subdomain. or those unresolved subdomain's are also important

       - ***You will get a http probed file as well. It resolved active and passive subdomains then pass it for permutation. That add all active passive and permuted result. And pass it for http probing. the subdomains for sub.txt all resolves. So you can work with their ip and ports. It's recommended to use this tool on vps at it will do hard active Enumeration***

         - Yes when i use it on my lapy i cant do anything other then sef

           - ***Yes if you run shuffledns with all.txt you will face this same. So use a vps for those type of recon stuff***