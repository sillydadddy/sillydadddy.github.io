---
layout: post
title:  "Infosec Bugbounty AMA with Syed Mushfik Hasan Tahsin"
categories: infosec-bugbounty-ama
excerpt : "AMA with Syed Mushfik Hasan Tahsin"
author: Gurvinder Singh
---

# AMA with [Syed Mushfik Hasan Tahsin](https://twitter.com/SMHTahsin33)

<br>

 ## 🔥 16 year old Bug Bounty Hunter 🔥 | ✨ Cyber Security Enthusiast ✨

<br>

 - Q1) What are burpsuite plugin you used?

 - Q2) How you learn new vulnerability?

 - Q3) Have you automated any vulnerability and how?

 - Q4) As a fresher what vulnerability to focus?

 - Q5) How to construct our own xss bypass payload?

   1. ***Use Mostly Used inQL for graphql Queries. Reflector v2, Paramminer, Collaborator Everywhere, Burp Linkfinder and Burp Secretfinder.***

   2. ***Take a Bug Class and search like "CSRF hackerone", "CSRF medium" It will give you a lot of Resources to read.***

   3. ***Nope I Didn't, But Sometimes Looks For RXSS with wayback + KXSS and have success with this.***

   4. ***There are nothing like that, You can start with anything. But bugs Like Idor and XSS seems less complex. You can got with them.***

   5. ***Constructing Own XSS payload isn't a matter. As [@zseano](https://twitter.com/zseano) says Don't Spray and Pray. Understand Whats going on. How's your input is being handled. Play with it and craft the payload as per need. That is of no use where it reflects inside href= and you are spraying tags.***

<br>

 - What got you interested in hacking?

   - ***When I Was In Class 5, From then i had an ambition to be a hacker. I Saw them on news (mainly the group anonymous), and got very interested in it day by day.***

   - ***Then Next year I started to get into this collect resources but in lack of proper guidelines I was Misleaded and did some random stuffs like 1-2years but didn't get any way into properly.***

   - ***Then in Ending of 2019 :) Started my journey with [@remonsec](https://twitter.com/remonsec) and some other people together. Started With SQLi and used to practice them on random sites. and Thus the interest of hacking rose in me more. Like Why Not? Not everyone can hack.***

   - ***and That's The Story Of Mine of Getting into Hacking.***

<br>

 - What is your hunting methodology for Recon process? Which is your niche bug (which type of bug you hunt most and focus on)? Any notes you can share?

   - ***Getting Most of the recon automated and after collecting the whole bunch of subs i go through them one by one and see the technologies in which. Then Start from the one that seems most interesting to me.***

   - ***It Depends, If the target has everything in it, Collect their ASN, Use shodan :) If has a CIDR, Scan it with amass, Collect subs doing passive,active,permutation enumeration and getting all of them through shuffledns for resolving them. Then i run content discovery on it.***

   - ***On that part i use GAU to collect urls, look for hidden params with arjun. Do Dir bruteforce, read JS and Collect endpoints from it via linkfinder and make a target based wordlist to fuzz it again with that.***

   - ***I mainly don't have any niche bug, but i find XSS more often.***

   - ***I Don't Usually Take Notes, If you need Notes on different bugs or ways and bypasses on them. You Can Check The Repo "How To Hunt" on [@KathanP19](https://twitter.com/KathanP19)'s Github: <https://github.com/KathanP19/HowToHunt>.***

<br>

 - How do you approach with a wide scope target (e.g recon)?

   - ***Wide Scope Means A Wider Chance To Recon. What You Can Basically Do Is. Collect The ASNs, You can use them in shodan. Scan The CIDR Ranges, You Can Use Amass for this. Look For The Org's Acquisitions like (facebook owns insta.whatsapp etc).***

   - ***After Collecting all the domains you could along with the Ip ranges. Run subdomain discovery on the domains. There are a lot of tools for The Passive one like Subfinder, Rapid7 FDNS, Assetfinder, Certspotter,assetfinder and more.***

   - ***For Active I Mostly use 'aiodnsbrute' along with [@Jhaddix](https://twitter.com/Jhaddix)'s all.txt. after collecting the result I concat this with the passive one and run 'dnsgen' on them to get the permutations. Then Just Run Shuffledns with resolver.txt and you are good to go with the alive domains.***

   - ***Then you have a lot of things to handle, you can run content discovery on them now, after probing them with httpx/httprobe. Check for subtakes with nuclei, do dir discovery, check them in 'gau' and get the urls.***

   - ***After Collecting these you can run any type of automations on them if allowed to and also test each manually.***

   - ***And Lastly, Check [@Jhaddix](https://twitter.com/Jhaddix) Recon Methodology V4. A Great Thing on Recon.***

<br>

 - Any path way? Any roadmap? I want learn but I don't find any Path?

   - ***If you are just starting. Start From The Basics of the things. Like Request/Response, Protocols, Web Technologies, Web Mechanism, Basic Networking. It's Essential For Getting Forward. Like if you know the basics, you can understand everything you read/see.***

   - ***If you don't have basics of these things, You mainly can't learn forward as the new terms you meet will confuse you and will eventually lead to a Demotivation.***

   - ***After you have the proper basics You can start learning differnt bug classes and go forward to test them. Learn and Gather Experience This Way. You Can Follow This, This is a Gem: <https://0xprial.com/how-to-get-into-bug-bounties-part-01/>.***

<br>

 - How to learn burp suite and amass? What is CIDR?

   - ***For Burp Suite, Just Stick With it and use the features one by one and you will get to know how it works. This also Worked For Me and if need more there are some Vids on it too. [@InsiderPhD](https://twitter.com/InsiderPhD)'s <https://youtube.com/watch?v=Ezs19sj04DU> is also awesome.***

   - *** For Learning Amass or any other tools like this, There might be not anything else better than it's docs itself. Also many tools have the -h or --help flag for getting the list of commands and also on how it works.***

   - ***These Questions Mainly Suites on Google. But as you asked, CIDR, which stands for Classless Inter-Domain Routing, is an IP addressing scheme that improves the allocation of IP addresses.***

<br>

 - How did you get into bug bounty? What are the resources you used to learn? What are some good online courses/yt channels to learn about bug bounty?

   - ***I Don't Usually Like To Do any Courses. You Can Learn Via Google and Youtube Through Random searches. I Started With This Blog by [@KHIZER_JAVED47](https://twitter.com/KHIZER_JAVED47), This Covered Up my most of the basics. This is really awesome: <https://whoami.securitybreached.org/2019/06/03/guide-getting-started-in-bug-bounty-hunting/>.***

   - ***For YT Channels You Can Look at Their Channels,***

     - ***[@stokfredrik](https://twitter.com/stokfredrik)***
 
     - ***[@NahamSec](https://twitter.com/NahamSec)***
  
     - ***[@InsiderPhD](https://twitter.com/InsiderPhD)***
  
     - ***[@codingo_](https://twitter.com/codingo_)***
  
     - ***[@Jhaddix](https://twitter.com/Jhaddix)***
 
   - ***They are really good.***

<br>

 - Why you Hunt?

   - ***To Learn and Experience mostly. Love to learn.***

<br>

 - How did you start bug bounty hunting?

   - ***Wanted To Be Hacker from a very long time which lead me to infosec :) Then Heard about the bug bounty. I Started Into this ready Writeups, H1 Reports and many more things. <http://whoami.securitybreached.org/2019/06/03/guide-getting-started-in-bug-bounty-hunting/>. This Blog Helped me a lot to cover up the basics.***

   - ***After That learnt some bug classes and started testing them on sites. and you Know about [@BugBountyHunt3r](https://twitter.com/BugBountyHunt3r). How helping it is to learn New Things and Experience in a Real World Environment. This thing also helps a lot. I Recommend it for everyone.***

<br>

 - Since when have you started learning? Have you started with SQLi? Want to know about your first bug finding. What kind of bug it was?

   - ***I Started Learning in the Starting of 2020. Talking of SQLi that's a very long story. This was the first bug I started learning With. If not in BB Websites, SQLI was the first bug that i found But The FIrst bug i got bounty for was a Full Path Disclosure, P5 mainly.***

   - ***Was in a RDP that's why they accepted that, but my suggestion will be not to report those now. Make the target high, and believe me it works good. Target P1, and you will be finding P2-P3.***

<br>

 - What useful information can I see about a target from the outside? (Enumerability)

   - ***There are many things you can find Passively.***

     - ***Do Github/Google Dorks, Who Knows What Might Leak.***

     - ***Search For URLs using GAU, Which utilizes wayback,otx and many. One Found Invoice of Customers being leaked via OTX. (so Recommended)***

   - ***and After Passive You Can Do Content Discovery on the website:***

     - ***Dir Bruteforce with common wordlists like common.txt from seclists.***

	 - ***Make Own Wordlist for the target from URL collected by wayback.*** 

     - ***Read JS Files for endpoints.***

   - ***(Can Be Automated With Linkfinder)***

<br>

 - How to keep my motivation after getting lots of bug are duplicate & N/A?

   - ***Dupes and N/A are natural process in bug bounties. I can't ensure you how can you ignore dupes. But While reporting somethin ask yourself "What can you do with it?" This might help you to be safe from N/As.***

   - ***And To Keep My self Motivated, I do Pick VDP and shot them. Find a couple of bugs and it recharge me. I also read writeups and reports which restores the confidence and I'm again good to go.***

<br>

 - Q1) For how long you have been hunting?

 - Q2) How long it took you to get into infosec?

 - Q3) What was your first bug?

   1. ***It's likely to be 1yr+ in infosec.***

   2. ***Took me 2-3 months to get a clear view on the basics and getting started.***

   3. ***If it's Non-Paid Bug that was a SQLi to be my first bug and got paid for a FPD a long ago. (This is p5) as that was rdp, they did accept it. But Clearly Don't Recommended Going for these now. Target higher and you will reach the height.***

<br>

 - Which bugs do you typically look for? What's your highest bounty? Favourite swag you've received till now?

   - ***I Don't Have any Specific Class Of Bug That I Look For. But I find XSS more Often.***

   - ***Just not wanting to answer anything to these as it won't be a point of learning or help anyone. Hope you can understand.*** 

   - ***Uhmm Got few. But I Like The [@BugBountyHunt3r](https://twitter.com/BugBountyHunt3r) Hoodie most.***

<br>

 - What was your daily time spent in the initial phase of entering into infosec/BB? How and what did you practice daily to be this good as you are today?

   - ***I am Still Learning At The Very Beginning I Used to spent like 7-8hours a day on learning. I took like 2-3 Months to cover up the basics. Then I used to take one bug class and read H1 Reports and Medium Writeups regarding that. and Then Used to practice in labs like websec.***

   - ***And After Doing some labs I used to look for the bug on mass targets. Gathering experience.***

<br>

 - How do you manage if your master of procrastination inside you is not letting you to work and making you feel dumb?

   - ***Watching and Reading Writeups on Different Types of bugs will charge you up. Doing Some CTF also works Good for me.***

<br>

 - How you stary motivated?

   - ***Motivation is a state of mind. You Can Read Writeups, H1 Reports, Watch [@stokfredrik](https://twitter.com/stokfredrik)'s Videos, [@NahamSec](https://twitter.com/NahamSec)'s Interviews. This Will Recover your lost confidence for sure. and Do What you like to do most. It will recharge you again for sure.***

   - ***Also Can Shot Some Wide Scopes VPDs, Getting some bugs on those are easier than on the Public BBPs. This Can Also Give you a good Feel.***

<br>

 - The amount of time you spent on recon vs hacking? Are you using any recon automation?

   - ***Most of the stuffs that I do frequently has been automated with bash. For example: Subdomain Enumeration.***

<br>

 - When you started hunting and what was your inspiration?

   - ***I Started a year back. My Biggest Inspiration into hacking was that they are cool. Not everyone can hack.***

<br>

 - Do I have to learn javascript for identifying and exploiting xss?

   - ***It's not obvious to learn JS for XSS. But helps in Identifying DOM Based XSS and might help in bypasses imo.***

<br>

 - You should find a bug within 5 minutes. Where would you look first?

   - ***GAU, Found a Lot of XSS through this. Also JS, It leaks many endpointssss.***

<br>

 - How to detect api-key in js file?

   - ***Open In Browser and You can Simply Search for them with keywords like "api-key", "api_key" or similar.***

<br>

 - What was your first bug?

   - ***The First Bug I Learned and got was SQLi But The First Bug I got paid for was a Low bug (Full Path Disclosure). That was a RDP site that's why they did accept but I don't suggest looking for these.***

<br>

 - What's an easy win bug you found and paid a bounty?

   - ***The XSS on a BugCrowd Program found with Wayback+KXSS.***

<br>

 - Have you any specific checklist that you follow?

   - ***No, I Don't Follow any specific Checklist till now But I think you can find one here <https://github.com/KathanP19/HowToHunt/tree/master/CheckList>.***

<br>

 - Does programming helps in bug bounty hunting?

   - ***Yeah, Programming Languages are not obligatory but knowing helps. I Learn't Bash and it really helps me for my automations.***

<br>

 - Any weird bug you reported which you are proud of?

   - ***Mostly I Hunt on my free time,not very often. But the Email Confirmation Bypass Found Recently was the weirdest one. I still have no idea how did it work.***

   - ***<https://twitter.com/SMHTahsin33/status/1383419073862660096/photo/1>***

<br>

 - What bug classes will you suggest a beginner?

   - ***I Find XSS a lot, So It's Better to with it. I Find it easy to discover.***

<br>

 - In which language you code often?

   - ***Bash - Shell Scripting.***

   - ***This Playlist is Great For Learning Bash: <https://youtube.com/watch?v=cQepf9fY6cE&list=PLS1QulWo1RIYmaxcEqw5JhK3b-6rgdWO_>.***

<br>

 - How you pick a target?

   - ***My Target selection is based on scope. As I Love To Recon mostly. I select targets With wider scope.***

<br>

 - What advice you will give people who want to start BugBounty?

   - ***Learn The Basics First. This is a thing everyone ignores and it becomes a great obstacle in their learning experience.***
