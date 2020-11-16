---
layout: post
title:  "Infosec Bugbounty  AMA with zseano"
categories: infosec-bugbounty-ama
excerpt: " AMA with zseano "
author: Ravi Shankar Gurram
---

# AMA  with [zseano](https://twitter.com/zseano)

<br>

## Bug bounty hunter, coder & mentor. Achieved #2 on [@Bugcrowd](https://twitter.com/Bugcrowd) from just 1 program, recognized by Amazon Infosec team. 800+ bugs submitted. Founder of BugBountyhunter.com

<br>

 - Any Advice for Beginners ?

   - ***try not to over-think things. take the site at face value as to how it works :) & write lots of notes!!***

<br>

 - What's the best methodology for beginners to start with?

   - ***hack for features! :) look at what's in front of you and test it how it should work and understand it.***
   
     - ***eg: it's a forum, you can login and post topics. first thing that comes to mind: upload images on topics, stored user content (xss), edit profile (idor), etc***

   - ***so based on that, as your testing the feature and you get some weird behaviour (you input &lt;img src=x onerror=alert(0)&gt; and it reflects <img>) you can then begin to read up on that specific issue.***

   - ***is the forum using third party software? is it markdown ? anyone discovered or had similar problems?***

   - ***try the most common, &lt;img onnotreal=&gt; (is it just blacklist filtering?), how does it handle other tags like <a href=java%0dscript:prompt\`0\`&gt;). and down the rabbit hole you go! more features, more to play, more bugs?? :) happy hacking***

<br>

 - What are the low hanging vulnerability which we can consider in begining.?

   - ***Personally i would read about the most common bugs (xss, idor, csrf, open url) and understand what they are, common bypasses (\/\/ for open urls for example). Then pick a program, test each feature and write notes on whats expected to happen, what you believe you can do, what's actually happening. what params are used etc. then you can say "oh okay, on this page i can see my param ?test= is reflected, so this may be xss" and you can spend further time learning/practising XSS. rather than \*just\* focus on one bug type***

<br>

 - Word of advice to the people who looks up to you?

   - ***never give up, and don't quit too early. patience & time! :)***

<br>

 - What should be the PC configuration for doing bug bounty hunting?

   - ***all you need to run is google chrome and something like burp/fiddler so it doesn't matter imo about the OS (windows or linux, both work fine). min ram i'd prob get 4GB to run burp (since it loves to eat it) but the rest you don't need anything special :) for tools use a droplet***

<br>

 - What is your favourite bug bounty CLI tool?

   - ***ffuf and aquatone :)***

<br>

 - What are the burp plugins you will be using?

   - ***i don't use any plugins tbh***

<br>

 - What is your favorite web vulnerability and methodologies/tips of that vulnerability?

   - ***No fav tbh.. I really enjoy hunting for issues that are caused from bad filtering (eg: webhook, they don't want you to hit 127.0.0.1 so they filter \*just\* that, so you try http://localtest.me)***

<br>

 - what are some of the tool you use for recon and what are the common/favourite bug you look for in a program

   - ***aquatone, amass, sublist3r, dnsgen.***
   
   - ***no fav bug tbh, and common would be the usual, xss, idor, csrf, open url, leaks (github etc) :) most sites vuln to the same stuff over and over again ;D***

<br>

 - Do you consider that Amass is one of the best reccon tool?? How to use Amass like a pro ?

   - ***amass is pretty good yes :) there's a great video on [@NahamSec's](https://twitter.com/NahamSec) stream here with [@jeff_foley](https://twitter.com/jeff_foley) on using amass efficiently - https://www.youtube.com/watch?v=H1wdBgY1rtg&ab_channel=Nahamsec***

<br>

 - How many languages u know specifically all web langs and python or golang?

   - ***just php tbh :/ not really confident in python or golang, but will probably learn one day :D***

<br>

 - Do u recommend learning any language like js, python or go?

   - ***depends on your intentions? learn js to build sites/understand why they used, python/go if you want to build tools :)***

<br>

 - What make a specific program pay your attention ?

   - ***Wide scope, lots to play with, various different integrations (diff teams, diff codebases). I like to hack on familiar names***

<br>

 - how do you pick a pgrm?

   - ***I like to test on sites I know the name of and i've used their site before (understand how it works)***

<br>

 - what are some common bugs which you always look for while hunting on a target which has all of its assets owned in scope?

   - ***common bugs for me would be open urls to leak something (usually try play with their login flows as much as poss, any mobile apps, third party integrations etc), xss , cors (if lots in scope, how do the sites 'talk' to each other etc), csrf and idor***

<br>

 - Any specific type of Endpoints on which one should keep an eye for finding idor...

   - ***any feature that looks like it's using some type of integer/id value to determine 'something'. /account/update/52 - 52 would be the ID to play with. (can depend on what the feature does whether it's a vuln or not, that's up to you work out when testing on the site :D)***

<br>

 - How did you approach (tools, methodology) API endpoints for testing?

   - ***depends how the api works, what does it do, what's its use, params used etc :) but typically i look for idors, using them to bypass 'filters' (once found desktop site filtered xss, mobile api did not) or leaking / manipulating info***

<br>

 - How to stay with one program and not switch ?

   - ***I like to hack on names i'm familiar with and understand how they operate. add in a big scope and lots to features and i'm yours for months :D Find yourself a program you \*enjoy\* hacking on.. you are interested in learning more and more as to how it works.***

<br>

 - What keep you motivated and not give up ?

   - ***I enjoy what I do :)***

<br>

 -  I have been in bug bounty for 8 months now. Pretty good with low level bugs but not able to land at that "critical bugs" zone. What should I focus on ? Any advice that you could give to me about this?

    - ***What type of bugs are you finding already? A lot of it can depend on the features available on web app, sometimes things like SSRF/XXE just aren't there (no matter how hard you look). If you think about criticals in web apps think about features they're found on***

    - ***For example***

      - ***rce -> file upload, exposed admin panel with some way to execute code, command injection on a param?***

      - ***ssrf -> developer portals to test webhooks, features that use urls (image uploads ?), etc etc***

      - ***it can all depend what's infront of you :) hope this helps***

<br>

 - r u huntin these days ? what is your full time job now ?

   - ***I do a lot of testing for companies that approach me privately. Right now i'm doing priv tests & running bbhunter. I will be starting to spend more time in bug bounties now i'm finding my two feet again :D***

<br>

 - r u doing BB full time? What progr. Languages do you know? For how many years have u been doing BBs?

   - ***I wouldn't say I do it full time personally as I typically dig my teeth into 1 program for a set amount of time and then I take some breaks. I am also doing more private tests for companies that approach me. When i'm active i'd say ~3-4months a year hacking on bb total time***

   - ***I haven't been active this year much due to making bb hunter but i'm getting back to it :) The only server side language i'm confident in is PHP, but I do web development also. I have been doing bug bounties since 2015 :)***


     - So it's not BBs 100% of the time. Good to know. It's probably nice being wanted by companies to help them out. Hope I'll get there too

        - ***I found an issue recently on a client test and they forwarded it to [redacted] (didn't realise affected all), who actually has a bb program. Co-ordinated with both sides and reported and got paid for it from bb program :) so BB and client tests can go hand in hand sometimes :D***

<br>

 - do u perform whitebox testing too ?

   - ***If any of the subdomains are using something like wordpress i will sometimes view the installed plugins code to have a peak as you may find something new that no-ones ever found :)***

<br>

 - Few business logic bugs that you'd like to mention?

   - ***In order to claim ownership of a property they would ring the number listed for the property with a unique code. However they released a new feature to buy ads for your property and I could buy ads for any property using sandbox cc and it added me as admin w/ no verification =]***

<br>

 - What are the most vulnerabilities to concentrate on for easy win? For example "Subdomain Takeover" and "SQLi" are rare nowadays, where as Account Take Over Techniques are much common.

   - ***Easy wins are prob some type of account takeover / sso token leakage via open url :) look on mobile apps for third party integrations (if available) :D***

<br>

 - What do you try to do when you come across a login page on any subdomain?

   - ***if i can't register then i will try hunt through what's available (any js files, what's in the html) and try find a way around the login. i'll try common logins (admin:admin), if it's third party software check for any past issues etc.***

<br>

 - What do you try to do when there is a blank page on any subdomain?

   - ***run wordlists to try find something***

<br>

 - How to get the valid parameters for a target?

   - ***Can be found when using their site. this is why i built inputscanner to scan sites for params they use. then jsscan to find even more***

<br>

 - How do we know if any parameter is valid for a url? Is there any shortcut or script to do this?

   - ***send a get/post req -> check in resp for anything to do with the value you used / anything different. intruder works fine***


