---
layout: post
title:  "Infosec Bugbounty AMA with Devansh"
categories: infosec-bugbounty-ama
excerpt: " AMA with Devansh "
---

# Projects by [Devansh](https://twitter.com/0xAsm0d3us)
 

## [Favfreak](https://github.com/devanshbatham/FavFreak), [ParamSpider](https://github.com/devanshbatham/ParamSpider), [OpenredireX](https://github.com/devanshbatham/OpenRedireX)

<br>

# AMA with [Devansh](https://twitter.com/0xAsm0d3us)
<br>

 - What is your opinion on the current bugbounty scene ? Are you aware of the different stake holders  and their behaviors ( for eg :-  ppl cashing out BB success to other fields like mentoring and courses ) What is ur suggestion for a new comer in BB who dreams for those $$$$ ?

    - ***I don't bother myself from thinking about bugbounty scene or what others are doing, It's better to be ignorant sometimes, and if someone is cashing out their BB success to other fields , Good for em,***

    - ***For people just starting with Bughunting, I just have one advise, don't compare yourself with others, rather compare yourself with your past self, measure your progress with your own parameters, not by the bars set by someone else***

<br>

 - As a Beginner, what to learn as (1, 2, 3..) to start in BB?
Example:

    1. ***First get yourself familiar with basic concepts such as HTTP/Headers/How browsers work/Borwser security mechanism, JavaScript basics , this is the most fundamental step, after this start focusing on specific vulns***

    2. ***This field is so vast, you can never learn each and everything, learn to prioritize things that you love (for ex: I love Unicode related stuff, that's why I pay most of my attention looking for Unicode normalization bugs)***

    3. ***use the knowledge/work done by other researchers as your entry point, then add your own research value to that special topic, soon you will fall in love with this learning process, and with persistence and patience, you will improve gradually***

<br>

 - Where did you learned and how you learned and what suggestions would you give for beginners based on your past

    1. ***is no one specific abstract source, you have to start at some point  from somewhere, Portswigger's web academy provides very well organized content (theory+labs), learning never stops, try to apply what you learn, otherwise learning is of no use!***

    2. ***I have only advice that I can offer , "you don't need to know everything", prioritize topics of your interest and dig deeper! Enjoy the learning process, the results will  definitely be positive.***

        - When you starting what bug you picked to learn and now what you suggest for beginners bro ...?
           
           - ***When I started , my focus was on business Logic issues, you can't automate em, and hence the chances of getting a dupe are very low, Ex : FB bug I reported last year that got paid $1000 https://www.youtube.com/watch?v=dvCc9WzOk-g&feature=youtu.be***


<br>

 - What are the mistakes you made that you would want any beginners to avoid?

    - ***you can never learn each and everything***
    - ***there will always be peeps better than you, don't compete , learn from em***

<br>

 - Do u advise a beginner to go and hunt in bug bounty platforms or just participate in CTFs and labs to gain thorough knowledge about the hacking scenarios? 
Which programming language do u think will be most useful for a beginner?

    - ***You can start with Real programs, start with programs that have less Competition (maybe a VDP?) , Python is very easy to learn, and it will be useful for you in long run!***

<br>

 - In your opinion, where should one start? Jumping directly into the BB programs or go for VDPs? If VDPs, could you please suggest some large scope VDPs?

    - ***Start with VDPs, then shift to BB programs , chose a program with large scope(ex: DoD, Sony, General Moters)***

<br>

 - learned mostly from paid resources or free resources?

    - ***I personally never took any paid course, there are a lot of free resources available, just a click/search away***

<br>

 - What was the motivation for making favfreak?

    -  ***I am using Favicon hashes as a fingerprinting technique from past 2 years now (credit goes to [@shodanhq](https://twitter.com/shodanhq))***

<br>

- What is your favourite vulnarability?

    - ***Favorite Vulnerability : Unicode normalization issues Reference: https://www.youtube.com/watch?v=hyyVeKdpeUU&feature=youtu.be***
<br>

 - When did you learn to code in python and had confidence to write such amazing tools?

    - ***I started learning Python when I was in 11th standard, Python is very easy to learn, if you are just starting with python, go through the books "learn python the hard way" and "Automating boring stuff with python"***

<br>

- Any advice for people who learning python programming? Learning approach you followed?

    - ***Python Resources for beginners :***
        - ***https://python101.pythonlibrary.org***
        - ***https://automatetheboringstuff.com***
        - ***https://ehmatthes.github.io/pcc/***
        - ***Black Hat python (Book)***
        - ***Violent Python (Book)***
<br>

 - Favorite vulns :
 
    - ***Unicode Normalisation Issues***
    - ***Information disclosure issues***
    - ***URL parsing issues***
    - ***IDORs*** 
    - ***Business Logic Flaws***

<br>

 - Favorite Python Libraries: 

    1. ***pwntools (for binary exploitation challenges in CTFs)***
    2. ***scapy (networking/packet related stuff)***
    3. ***asyncio + aiohttp (for asynchronous programming)***
    4. ***Tensorflow (for Machine learning stuff)***

<br>

- Which program I hunt most?

    - ***Facebook***

<br>

 - can you explain your methodology in brief ?

    - ***I don't follow any specific methodology, Its just me, trying wierd things, sometimes those wierd things lead to unintentional behaviors, and then I dig further, with experience and persistence you start to see patterns, that's about it***

        - do you hunt on the root domain or go for the sub-domains, and how do you select one subdomain from thousands subdomains
            
            - ***I hunt on main app, get yourself familiar with the functionalities, prioritize the features that look fishy(involve some kind of access controls), try to circumvent those controls, then go for subdomains and other assets !!***

<br>

- What tools you use for subdomain enumeration?

    - ***amass, Subfinder, OneForAll, dnsgen(for alterations and permutations), massdns(for resolving), some custom tools for Extracting DNS records from TLS/SSL cert***

<br>

 - Can you tell your recon steps

    - ***For me, recon is a never-ending process, and I run my tools almost 24x7 (continuous asset monitoring and profiling You can refer to this awesome article: https://offensity.com/de/blog/just-another-recon-guide-pentesters-and-bug-bounty-hunters/***

<br>

 - What all are tools you use for recon?

    - ***Tools I use almost daily :***
        - ***masscan***
        - ***nmap***
        - ***massdns***
        - ***Favfreak***
        - ***httpx***

<br>

 - How to find juicy information from  GitHub source of an application.

    - ***Tools I use for this purpose:***
        - ***[Git-hound](https://github.com/tillson/git-hound)***
        - ***[Gitrob](https://github.com/michenriksen/gitrob)***
        - ***[Trufflehog](https://github.com/dxa4481/truffleHog)***
        - ***[shhgit](https://github.com/eth0izzle/shhgit)***

<br>

 - How can we find information disclosure other than github dorks and js files

    - ***I use signature-based scanning (you can find the signatures from here https://github.com/eth0izzle/shhgit/blob/master/config.yaml), crawl the URLs (using \`meg\` or \`httpx\`), store the responses, match the responses against these signatures, that's about it***

<br>

 - How will you proceed for XSS if you find open redirect in Google??.... Also, what other bugs you may try specific to google

    - ***Open redirect to XSS is not always possible, it depends on the context(where our payload is getting reflected), in some cases something like this should work \`url=javascript:alert(1);\` [context: <a href=\"javascript:alert(1);\">click</a>]***

    ![](../images/devansh ama example screenshot.png)

    - ***But you shouldn't report Open Redirects(when analyzed severity and impact on CVSS scale, the severity is almost negligible), Open redirects are great for chaining multiple bugs (say: SSRF/CSP Bypass)***

        - Yes, that's a generic thing. I have just started hunting on Google. Not much aware of it. I thought you may have hunt on this target before and could provide more target specific attack Vectors.

            - ***Google doesn't accepts open redirects so don't report em right away, and tbh there are no secret techniques, Keep on trying wierd things to trigger unintentional behavior, and where there is an unintentional behavior there may be an underlying security issue***

<br>

 - How you look for Sensitive Data exposure? 
 
    - ***For sensitive data exposure, I use signature-based scanning (you can find the signatures from here https://github.com/eth0izzle/shhgit/blob/master/config.yaml), crawl the URLs (using \`meg\` or \`httpx\`), store the responses, match the responses against these signatures,***

<br>

 - How you manage to bypass 403 authorization header missing page and Forbidden page?

    - ***For Bypassing 403 pages, you can try a bunch of things :***
 
        1. ***X-Original-Url: /admin (URL rewrite sometime leads to 403 bypasses)***

        2. ***Improper URL parsing can also lead to Auth bypasses(refer to this https://youtube.com/watch?v=voTHFdL9S2k)and the list goes on and on***

<br>

