---
layout: post
title:  "Infosec Bugbounty AMA with Mohd Waseyuddin"
categories: infosec-bugbounty-ama
excerpt : "AMA with Mohd Waseyuddin"
author: Gurvinder Singh
---

# AMA with [Mohd Waseyuddin](https://twitter.com/waseyuddin)

<br>

 - Q1. How you manage your time while you were beginner (learning hacking) and how much time you gave to learn and hack?

 - Q2. After how long you got your first valid and bounty and which was your first bug?

 - Q3. Last but not the least, any tips for not beginner but not pro also?

   - ***Starting is tough for every researcher. In the beginning I didn't have access to internet so In the college I used to download blogs YouTube videos and come home learn the concepts and take notes. First I learn and then I hack So 50% time of learning and 50% for hacking.***

   - ***It took 3 months to get my first valid bug and please check my previous answer regarding the information of my first bug.***

   - ***Start with portswigger and pentesterlab and try the same on live target's.***

   - ***In the beginning you will be welcomed with a lot of duplicates,NA,informatives so kindly accept it without getting demotivated.***

   - ***Read blogs writeups and check out the new CVEs.***

<br>

 - What tools do you use? What burp suite plugins do you use?

   - ***Tool I use Amass,Subfinder,Subjack,Httpx,nuclie,Waybackurls,Naabu(quick port scan),Sqlmap. For collective recon, I use magic recon <https://github.com/robotshell/magicRecon>.***

   - ***Burpsuite Plugins I use active scan ++,Bypass Waf,Collaborator Everywhere,J2EE scan,param miner.***

<br>

 - Q1. First bug? How long did you take to find it?

 - Q2. Which is your Favourite bugbounty platform?

 - Q3. Which is your favorite bug type annd methdology for finding it?

   1. ***First Bug "leaked credentials via Github Repository"(reported with exploitation and good impact). For more information you can read an article for my good friend: <https://orwaatyat.medium.com/your-full-map-to-github-recon-and-leaks-exposure-860c37ca2c82>.***

   2. ***Bugcrowd is the only platform I report bugs and is my favourite bug bounty platform: <https://orwaatyat.medium.com/your-full-map-to-github-recon-and-leaks-exposure-860c37ca2c82>.***

   3. ***Authentication Bypass. All the authentication-related bugs I've found are through shodan. It's a pure treasure. Give it a try. You can use this Dork .and discover a lot ssl:"target" 200 http://Ssl.cert.subject.CN:"target.*" 200***

     - ***It will fetch all the ips which has SSL certificate of target and which has 200 response code. You also get some IPs which are not meant for public or is for internal purpose some dashboards even with out authentication.***

<br>

 - Can you share some tips regarding SSRF?

   - ***This should cover almost all tips: <https://twitter.com/search?q=bugbountytip%20ssrf&src=typed_query>.***

<br>

 - Q1. Do you use any other complete recon tool other than magic recon?

 - Q2. What is your suggestions regarding prettyrecon?

 - Q3. For a beginner, which complete tool would be best for recon?

 - Q4. Do we have to buy VPS for recon is there any way to get it for free?

   1. ***I usually use both pretty recon and magic recon.***

   2. ***It's worth trying( if you have some bounties in your pocket), sensitive file disclosure and CVE scan are good features.***

   3. ***Use all the tools of Project discovery.***

   4. ***If ur target has huge assets then you can try VPS else a basic laptop should the work.***

<br>

 - How to subdomain takeover via cloudflare?

   - ***I believe Subdomain Takeover via Cloudflare is not possible anymore. I tried a couple of times but didn't succeed. You can refer to this for more information: <https://github.com/EdOverflow/can-i-take-over-xyz>.***

   - ***<https://aws.amazon.com/blogs/networking-and-content-delivery/continually-enhancing-domain-security-on-amazon-cloudfront/>.***

<br>

 - Any weird bug you reported which you are proud of? Your 3 most favourite tools? Your favourite public program?

   - ***Found an IP of the target through shodan when visiting the IP displays drupal installation setup(reported without installing the setup). Although this asset was out of scope the target paid $$$.*** 

   - ***Github, Shodan, Nuclei.***

   - ***Private programs are my Favourite.***

<br>

 - While enumerating hidden directories I got mostly 403 response code so what you do after enumerating hidden directories and tools you used?

   - ***This tool covers almost all bypasses. Give it a try: <https://github.com/iamj0ker/bypass-403>.***

<br>

 - Which tool do you prefer for checking subdomain takeover subjack or Nuclei or subover?

   - ***I use subjack for checking subdomain takeover.***

<br>

 - Can you tell me which and tools and extensions you use for finding sql injection including the burp plugins? Any good resource to start for sql injection?

   - ***Tool I use for sql injection is SQLmap and burp plugin as CO2. Give a try to portswigger and pentesterlab labs. That's the best resource I know.***

<br>

 - How you do github recon?

   - ***Here is the article with full explanation: <https://orwaatyat.medium.com/your-full-map-to-github-recon-and-leaks-exposure-860c37ca2c82>.***
