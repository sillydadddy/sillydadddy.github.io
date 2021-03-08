---
layout: post
title:  "Infosec Bugbounty AMA with Sunil Yedla"
categories: infosec-bugbounty-ama
excerpt : "AMA with Sunil Yedla"
author: Gurvinder Singh
---

# AMA with [Sunil Yedla](https://twitter.com/sunilyedla2)

<br>

 - Recently you tweeted about CSRFs...wanted to ask if you see an endpoint that uses JSON how do you try for CSRF there?

   - ***For endpoints that use "json" in request body, use "xmlhttp" format. use "setRequestheader" to force add any header that is required. Sometimes system will restrict the users for "Content-type" as well, to bypass that this is good article: <https://blog.appsecco.com/exploiting-csrf-on-json-endpoints-with-flash-and-redirects-681d4ad6b31b?gi=66298e69a0ea>.***

<br>

 - I have some problem...I can't report so many bugs with manual huntingbut how you are managed to find so many bugs..... Any tips from your experince?

   - ***Like I always say don’t focus on regular known bugs try to find unique bugs. You just need to understand how the feature is working and then start breaking it in all possible ways.***

<br>

 - Do you do android testing?

   - ***Nope but I have to.***

<br>

 - Please explain the approach of you towards CSRF and tips to bypass CSRF.

   - ***I consider myself still as learner but for csrf check patiently for all endpoints, there are certain tricks to bypass csrf will try to create a list and post in future but key is to patiently rest all endpoints and don’t stop when you see csrf header.***

<br>

 - How you approach CSRF vulnerability? Which tools you use in daily recon process? Some tips for Business logic bug?

   - ***I check almost every endpoint, most cases we ignore once we see strict CSRF protection but newly added endpoint might be missing sometimes.***

   - ***Subfinder, dirsearch, waybacktool.***

   - ***Understand the functionality and go with pass/fail scenarios.***

<br>

 - What are the most common bugs that you encounter? Tips for CSRF and most common CSRF bypass that you use? Tips for SSRF and IDOR?

   - ***Most common bugs would be BAC, Authorization bugs, CSRF.***

   - ***Go deep, if you csrf header doesn’t mean it’s protected, check all endpoints I can essere you atleast 1 endpoint will not be protected with CSRF. It’s all about patience.***

<br>

 - Bugcrowd vs HackerOne?

   - ***Very tough question bro..both are good!but if you are a beginner I would suggest you to go for Bugcrowd, they still accept few P4 bugs which Hackerone doesn’t accept.***

<br>

 - Which are the guideline, resources and toolset behing you success?

   - ***Resources: I mostly rely on medium and Hackerone hacktivity.***

   - ***Toolset: I’m not automation guy but I use tools like: Subfinder, waybacktool , dirsearch for little recon.***

   - ***Guidelines: If I was working ill not worry about bounties, I make sure I find atleast 1 loophole.***

<br>

 - How to find bugs consistently and how do you find it? How to find valid bugs quickly as a beginner, what would you suggest to younger you that how you hunt?

   - ***To find consistent bugs you need to create your methodology. Try to find more unique bugs, it’s okay if it’s low priority but still it should come from your own methodology.***

   - ***Don’t expect bugs will be found quickly. Tweets you are seeing “I found bug in 5 mins” may not happen everytime. Finding a good but will take time but it’s worth it. Just enjoy the journey of learning infosec stuff, trust me even if gets bounty or not that helps you get a job!***

<br>

 - Should I learn coding basics before getting into bug hunting?

   - ***Trust me brother coding is not required in the initial days, little basics of JS and HTML will be enough. But yeah coding is always an added advantage.***

<br>

 - How you hunt SSRF?

   - ***Simple and straight during your testing, anywhere you see Input box to enter URL or image upload(SVG file with malicious content) test for SSRF. If you get ping requests to your server, now you try to build the impact!***

<br>

 - Q1. Your favorite bug?

 - Q2. Your favorite program?

 - Q3. Most common CSRF bypass you have came across?

 - Q4. How often you found CSRF with JSON data?

 - Q5. Best tool or extension you are using?

   1. ***CSRF, OAuth related bugs, BAC.***

   2. ***Hellosign(now merged with Dropbox) they have excellent response time.*** 

   3. ***Removing CSRF header/accepting any value.***

   4. ***Many times, unfortunately most of us ignore when we see Json data.***

   5. ***Waybacktool is a good one!***

<br>

 - When you started how did you manage to fight imposture syndrome and how much  time you gave to bug hunting and learning in your initial days and now?

   - ***I keep a goal to read atleast 1 cool bug everyday. It could be very low priority but you should learn something new.***

<br>

 - When did you start hunting? What does it take to become a great bug hunter?

   - ***I’ll post a separate tweet of how I started BB and what made me start. I’ve started 4 years back but I’ve been serious since last 1-1.5 years. Patience and don’t give up nature.***

<br>

 - What are the common places to find http request smugling bug? Any tips about this bug?

   - ***Honestly brother I never found this bug yet. Thanks for asking this im gonna start diving deep into this from today!***

<br>

 - How you choose which medium articles & hackerone reports should you read?

   - ***I mostly search for it, let’s say I was stuck with csrf protection header, I’ll simply search for possible ways to bypass that header. Additionally You can follow channels like infosec community, this channel consists of bug bounty reports. I’ll try share the resource links.***

<br>

 - Where to try for SSRF and how you select a program to hunt?

   - ***Image upload, HTML rendering, HTML to other file type conversions, open redirect. Eventhough I’m not a recon guy I love programs with wide scope and many functionalities.***

<br>

 - How much time do you spend on bug bounty? How to take care of eyes while hunting?

   - *** I don’t have fixed time, but if the regret is interesting then there are no bounds.***

   - ***Take random break or use UV protected glasses.***

<br>

 - How to hunt for P1s like SSRF or RCE,etc?

   - ***I'll be honest brother, I didn’t find too many P1’s so I don’t wana fake that I know everything, but 1 suggestion I can give you is one should stick to a program for long to get P1’s, I went close to these and got dups!***

<br>

 - What you do when you didn't find a single bug in a day?

   - ***I simply take a break, never push too much coz you deserve a break too. Eat some nice food, watch good movie then back to work: read some good content,start working on VDP’s/daily usage apps. This helps you with fresh start, that works for me everytime!***

<br>

 - Which program to hunt as a beginner?

   - ***I would suggest you to hunt on websites which were created especially for testing purpose. For example, DVWA or portswigger labs.***

<br>

 - How do you manage your time when you were at the beginning stage?

   - ***In the beginning state without any methodology I kept working and resulted in 0 output later created my own methodology and started working on it. Also take enough breaks so that I don’t feel stressed. You can go for dual booting but make sure that it doesn’t impact performance.***

<br>

 - Any weird bug you reported which you are proud of?

   - ***I’ve recently published a writeup on this: <https://sunilyedla.medium.com/information-disclosure-through-signup-endpoint-86d2d66dfef1?source=linkShare-17732dfb2914-1613399344>.***

<br>

 - How can we find SSRF vulnerability and how can we find RCE where it is majorly found?

   - ***To my knowledge I found SSRF mostly at image upload, HTML rendering, HTML to pdf conversions, open redirect etc.***
