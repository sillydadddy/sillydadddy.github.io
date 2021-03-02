---
layout: post
title:  "Infosec Bugbounty AMA with Shubham Shah"
categories: infosec-bugbounty-ama
excerpt : "AMA with Shubham Shah"
author: Gurvinder Singh
---

# AMA with [Shubham Shah](https://twitter.com/infosec_au)

<br>

 - Where do you see bug bounty in coming five years?

   - ***I expect to see large corporations similar to Verizon really take their security seriously, and I hope, for the both of us, that bounty amounts continue to increase, not  decrease but that’s hard to predict. I see automation being even more prevalent. I see more esoteric bugs.***

<br>

 - Can you give me your private resolvers lists?

   - ***I recommend you take a look at DNSValidator from [@vortexau](https://twitter.com/vortexau) https://github.com/vortexau/dnsvalidator, there is also this project which constantly runs this and saves a list of working resolvers back to its repo: https://github.com/janmasarik/resolvers - you can always build something similar.*** 

<br>

 - Your approach to finding/looking for an SSRF? I mean what functionality you'd usually go after, like this might be useful and this is a false positive.

   - ***I’m usually looking for any functionality that may require outbound communication. I move through assets quickly, while trying to cover as many features as possible, with the aim of finding server side issues. Stop looking for client side issues and focus + content discovery.***

<br>

 - Is it possible to achieve 10k rep on [@Hacker0x01](https://www.hackerone.com/) who are starting bug bounty in 2021 and are ready to provide full time and dedication? How much investment(monetary) is required in crowdsourced pentest aka bug bounty for learning materials and toolset?

   - ***I promise you that its possible but it requires dedication and persistence. My posts on 120 days 120 bugs and Hacking Bug Bounties for Four Years goes into detail about how I was able to get to the position I am in on HackerOne: https://shubs.io/high-frequency-security-bug-hunting-120-days-120-bugs/ and https://blog.assetnote.io/2020/09/15/hacking-on-bug-bounties-for-four-years/.***

<br>

 - What is the best script for recon automation and your methodology for recon and hunting?

   - ***Subfinder is pretty great: https://github.com/projectdiscovery/subfinder. Also, consider getting access to SecurityTrails - http://securitytrails.com [@ChrisUeland](https://twitter.com/ChrisUeland) and his team have done an excellent job at collating data needed for recon. I can't fit my methodology in a tweet, but check my previous blogs.***

<br>

 - What's your approach on hacking aspx extension?

   - ***I try to see if debug mode is enabled and perform a lot of content discovery + IIS shortname scanner. Once I find an interesting endpoint, I fuzz it to produce error messages and disclose some source code. Otherwise, I try my typical attack vectors against it until it breaks.***

<br>

 - Any tips for content discovery?

   - ***Build your wordlists over time and add to them constantly***

   - ***Look for weird application behaviours (i.e. redirect to internal host)***

   - ***Bruteforce every subdirectory until there's nothing left to brute***

   - ***Print to terminal in colour mode (ffuf -c)***

   - ***Don't miss any spots***

<br>

 - Any resources for more on that IIS hacking?

   - ***I plan to make more videos on IIS next year. Until then, read the blog posts from [@irsdl](https://twitter.com/irsdl), he is someone I look up to when it comes to hacking .NET/IIS - https://soroush.secproject.com***

<br>

 - When did u start u hacking career? When did find ur first bug?

   - ***I started when I was 13, I found my first critical bug for a bug bounty at 14 (SSRF in BillMeLater PayPal).***

<br>

 - According to you, what are the popular bugs to find right now?

   - ***I don't really think about bugs being popular or unpopular, but I like to focus on server side bugs these days.***

<br>

 - If I want to sharp my skills on penetration testing and be a bug bounty, give me some basics to focus on and some advice from an expert's point of view.

   - ***Focus on server side issues and try and learn as many high/critical risk bug classes and how to find them as possible: http://projects.webappsec.org/w/page/13246978/Threat%20Classification.***

<br>

 - What was the motivation/story behind starting [@assetnote](https://twitter.com/assetnote)? What will be your advice to your younger self who just got to know about bug bounty and starting that path? What are the typical time duration you spend on a program, do you look for high priority bugs at the start?

   - ***I was automating bug bounties at scale and lots of companies asked if there was an enterprise offering. There wasn't one at the time, so we built it.***

   - ***Don't compare yourself with others, you are unique.***

   - ***Sometimes few hours, sometimes few weeks, depends on the interest.***

<br>

 - How you choose program Scope based or as per mood? Your favourite tool for recon? Tips for SSRF?

   - ***There are programs that I like to stick to (for example Uber), because I have spent a lot of time understanding their attack surface and can find new vulnerabilities quickly. No favourite tool for recon, focus on methodology instead. I am back on the newest version of Burp. I've switched back to this version because of 1) extensions that require it and 2) because I had some projects that I couldn't open in 17.***

<br>

 - How to find hig severity bugs like sqli rce and others wand what methodology we need to find such bug? Is it worthy to test every single parameter present in a request body with all kind of payloads like xss sqli rce ssti or we should test certain prameter only?

   - ***Understand how the application works and what it is doing with those parameters as much as possible before testing it for specific bug classes. Attempt some cursory payloads to test the behaviour of the application and then test it further based on that.***

<br>

 - What bugs to look at and approach when the scope is too limited (only 2-3 domains)?

   - ***Look very closely at the JavaScript, understand how API calls are being made and whether or not you have tested all APIs. Look for hidden or administrative functionality within the JavaScript. Perform thorough content discovery.***

<br>

 - Do you do content disc on all of the collected host or it depends on some factors?

   - ***There are "indicators" that tell me if I should spend more time on an asset. For example, I will be spending a lot more time on an asset with a PHPInfo file exposed because it indicates that the due diligence has not been done and theres more bugs.***

<br>

 - Is there any Defcon/Online talk/whitepaper/blog which provides good samples on content discovery and doing directory bruteforce the right way?

   - ***Nothing super specific to content discovery, but tangentially, related to recon: https://docs.google.com/presentation/u/1/d/1PCnjzCeklOeGMoWiE2IUzlRGOBxNp8K5hLQuvBNzrFY/view#slide=id.p.***

   - ***https://youtube.com/watch?v=GxkuBFUfnL8***

   - ***https://youtube.com/watch?v=C85ZOJgufuw***

<br>

 - Is subdomain takeover still worth to look manually/semi-automated? Any tips, methodology to detect subdomain takeover effectively? (I read patric,edoverflow,frans rosen but still not cleared up). If scope is small is it worth bruting subdomains and checking takeovers?

   - ***Yeah, for sure it's still worth looking for, but it's best you automate this process. You don't have to work too hard to get started, there is an OK Nuclei template for subdomain takeovers: https://github.com/projectdiscovery/nuclei-templates/blob/master/subdomain-takeover/detect-all-takeovers.yaml.***

<br>

 - Mistake you did while getting started? Best advice you would like to give to your younger self?

   - ***Focus on as many bug bounty platforms as you can***
 
   - ***Don't be afraid to fail***
 
   - ***Don't get complacent***
 
   - ***Invest more time into engineering, pentesting is not everything***
 
   - ***Publish more content and speak your mind***

<br>

 - What's your methodology on hacking small scope and large scope sir?

   - ***Small scopes, I go through the application thoroughly and read a lot of the JavaScript that powers the application, recreating API requests and fuzzing them. Large scopes, I move through assets quickly, performing a lot of content discovery to look for interesting behaviours.***
