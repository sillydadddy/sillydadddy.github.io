---
layout: post
title:  "Infosec Bugbounty AMA with Imran Parray"
categories: infosec-bugbounty-ama
excerpt : "AMA with Imran Parray"
author: Gurvinder Singh
---

# AMA with [Imran Parray](https://twitter.com/imranparray101)

<br>

 - What programming languages do you suggest for bug bounty hunters?

   - ***You can code in whatever language you want, But here are some of my favourite:***

     - ***Python*** 

     - ***Bash***

     - ***Golang***

<br>

 - Should I chose subdomain takeover as my first bug?

   - ***Start with anything easy, Don't start with bugs that are complex to find, IMO, Why Not IDOR?***

   - ***I would say look for issues like CSRF,CORS,Broken Access Control,Open Redirects etc.***

<br>

 - What are the methods to find admin panel and bypass it? If you find http request smuggling bug in site means.. How do you escalate it??

   - ***Finding Admins Panels:***

     - ***Google Dorks***

     - ***Wayback URL's***

     - ***Github Recon***

     - ***Bruteforce [dir/dns]***

   - ***Request smuggling can be escalated to many other issues like Account takeover, Token Leakages, Session hijacking and many more stuff, It purely depends upon the context of the attack.***

<br>

 - What's your methodology for small scope?

   - ***𝐔𝐧𝐝𝐞𝐫𝐬𝐭𝐚𝐧𝐝 𝐭𝐡𝐞 𝐩𝐮𝐫𝐩𝐨𝐬𝐞 𝐨𝐟 𝐀𝐩𝐩(𝐧𝐨𝐧 𝐭𝐞𝐜𝐡𝐧𝐢𝐜𝐚𝐥)***

     - ***At this point the I will try to figure out what is the purpose of app, For example google forms is used for collecting responses and doing some basic surveys and pools etc.***

   - ***𝐔𝐧𝐝𝐞𝐫𝐬𝐭𝐚𝐧𝐝𝐢𝐧𝐠 𝐭𝐡𝐞 𝐚𝐩𝐩(𝐓𝐞𝐜𝐡𝐧𝐢𝐜𝐚𝐥𝐥𝐲)***

     - ***At this point I try to figure out how things work technically Example: what kind of info is being published about forms and Do the target app have access control model or any kind of technology like markdown.***

   - ***𝐔𝐧𝐝𝐞𝐫𝐬𝐭𝐚𝐧𝐝𝐢𝐧𝐠 𝐡𝐨𝐰 𝐭𝐡𝐞𝐲 𝐝𝐨 𝐢𝐭***

     - ***At this point I look into several feature separately and try to understand how they have implemented them, For example in google forms How does they make forms public and private and How does the export feature work etc.***

   - ***𝐂𝐫𝐞𝐚𝐭𝐢𝐧𝐠 𝐀𝐬𝐬𝐮𝐦𝐩𝐭𝐢𝐨𝐧𝐬***

     - ***At this point I will create several assumptions about many things in the app, For example if the form is public can we still send a response via HTTP requests, Can we choose an out of range option in poll if yes what can go wrong.***

   - ***𝐀𝐭𝐭𝐚𝐜𝐤𝐢𝐧𝐠 𝐭𝐡𝐞 𝐚𝐩𝐩***

     - ***At this point I will use all of my assumptions that can create abnormal behavior in the app, For example Can we choose an out of range option in poll if yes can I distort the whole response data which is being already collected.***

<br>

 - Q1. Favorite bug you found?

 - Q2. What bug took you time to execute/escalate?

 - Q3. Favourite tools and plugins?

 - Q4. If you are going to choose a program to hunt for rest of your life, what would be that?

 - Q5. What will be your message for your younger self starting his journey?

 - Q6. Proud purchase?

   1. ***Integration-Hijacking.*** 

   2. ***HTTP request smuggling leads to account takeover.***

   3. ***ffuf | nmap | Autorizer | MadMethods | httpx | nuclei***

   4. ***It's a private Program.***

   5. ***Be persistent | Learn building things | Be a master on one thing***

   6. ***Recently bought a real estate property worth $55k.***

<br>

 - Can you share your approach to find HTTP request smuggling?

   - ***I personally use "Request Sumggler" Burp extension by "James Kettle."***

   - ***Cache Deception:***

	   1. ***You found an endpoint /user.php.***

	   2. ***Sends /user.php/imran.png -> check if it returns some sensitive content in response.***

	   3. ***Now copy the same URL and open it another browser browser.***

	   4. ***If you are getting served exactly the same content you saw in your previous browser, it's vulnerable to cache deception attack.***

<br>

 - What is your favourite program that you would love to hack?

   - ***It's a private program. and I have found more than 100 bugs and got paid $75k on that single program.***

<br>

 - What type of bugs would you mostly look for in public programs to avoid "duplicates"?

   - ***Spend more time looking for Logic issues, Most of the people aren't even looking for them.***

   - ***Spend more time on complex parts of application like integrations, Webhooks, Access control models and Role based Access controls.***

<br>

 - Burp extensions you use?

   - ***Autorizer***

   - ***Autorepeater***

   - ***HTTP Request Smuggler***

   - ***Logger++ / FLow***

   - ***JSON decoder***

   - ***Copy as Python Request***

   - ***Turbo Intruder***

   - ***Reflector***

<br>

 - Do you automate SSRF? Any suggestions to approach?

   - ***You can do that same stuff on Application level:***

     - ***Save burp History***

     - ***Grep all Endpoints***

     - ***Replace all Params with Burp-Collaborator***

     - ***Watch the Collaborator-client for pingbacks***

<br>

 - What would you suggest to someone who’s not finding a single bug?

   - ***Become the master of one bug.***

   - ***Start Building websites/webapps/MoboApps etc.***

   - ***Be persistent, Even if you can't find anything for weeks.***

   - ***Make a proper methodology of each bug which include:***

     - ***Where to look for that bug.***

     - ***How to Look for that bug.***

   - ***Don't loose hope.***

<br>

 - Web building/making mandatory if we new in bug hunting?

   - ***It's not mandatory, but it worth it and it good to have clearly/clean understanding of things before you start breaking them and the only way to have clear understanding of things is by making/building them.***

<br>

 - Google dorks which you mostly use?

   - ***Being honest, I rarely use google for searching anything sensitive, I think wayback is more hacker friendly than google.*** 
