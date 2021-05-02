---
layout: post
title:  "Infosec Bugbounty AMA with Neha Tariq"
categories: infosec-bugbounty-ama
excerpt : "AMA with Neha Tariq"
author: Gurvinder Singh
---

# AMA with [Neha Tariq](https://twitter.com/nehatarick)

<br>

 - Q1) What resources did/do you follow in your bug bounty journey?

 - Q2) What's your methodology when you approach a target?

 - Q3) Which programs and platforms do you hunt on and why?

   1. ***Resources:***

      - ***Web Security Academy by Portswigger***

      - ***CTF Challenges***

      - ***Online Articles on Bug Hunting***

      - ***Github for payloads, tools and many more***

      - ***Twitter community for daily tips and motivation***

   2. ***If it is a single website then I look at all the functionalities it contains, parameters, user roles, authentication system, and technologies being used. Then try to fuzz/test all the parameters for Xss and content injection, use "Autorize" plugin for IDORS, use SQL injection payloads manually for any error or response length changes and if I get something suspicious then run SQLmap for more testing. Likewise, I do testing for other bugs. But, if it contains a wild scope, then RECON process starts with subdomain enumeration, gathering old URLs with "waybackurls" by Tomnomnom, filtering data with custom one-liners and then approach every domain like I do normally.***

   3. ***Initially, I used to hunt via HackerOne platform, but due to my studies I could not be able to devote my time as much as possible. But, now after Synack I am getting extra serious towards my work and nowadays only hunt on Synack's targets.***

<br>

 - What is your hunting methodology? Which is your niche bug (which type of bug you hunt most and focus on)? Any notes you can share?

   - ***Check out all the functionalities, fuzz, got any error or unexpected behavior, then dig deep into it, try to chain bugs for high impacts.***

   - ***Nowadays, XSS but in general IDORS or business logic bugs.***

   - ***Sorry, but, right now I do not have any compiled notes of mine, but you should check out the following resources:***

     1. ***Pentest Book by six2dez***

	 2. ***Learn365 by Harsh Bothra***

<br>

 - Q1) Any favorite bug you found?

 - Q2) What bug took you time to execute/escalate?

 - Q3) Favourite tools and plugins?

 - Q4) If you are going to choose a public program to hunt for rest of your life, what's that?

 - Q5) What will be your message for your younger self starting his journey?

 - Q6) Proud purchase?

   1. ***Dumped full Database using Boolean Based Blind SQL injection with the help of SQLmap.***

   2. ***Almost 4-5 hours in a HackerOne's CTF challenge where I manually extracted the credentials using Boolean Based Blind SQL injection.***

   3. ***Burpsuite.***

   4. ***Maybe Google because of its wide scope, but, I am not sure that I will stick to one program for the rest of my life because I always like to hunt on new programs every time.***

   5. ***Be persistent, trust yourself and the potential you have, don't jump into conclusions before the end result.***

   6. ***My Laptop.***

<br>

 - Do you find low hanging bugs? If yes,how do you change your methodology from low to high?

   - ***Yes, I do find them often, but I tend to not report them every time until I chain them successfully to raise its impact. A perfect example to turn a low impact vulnerability to a higher one is this: <https://twitter.com/osiryszzz/status/1378540350281687044>.***

<br>

 - Methodology to find any XSS?

   - ***Simple workflow would be like:***

   - ***Gather URLs using gau + Burp Suite history ➡ Filter only parameter ones ➡ run Kxss or Dalfox with xsshunter ➡ If lucky enough you will get a reflective XSS.***

   - ***But, for the stored ones try to submit payload in each parameter you find during test.***

<br>

 - If you find out that there is subdomains takeover possible, which can be false assumption. To confirm it that yes! It can be takeover so what you do to confirm it?

   - ***I generally use Sudomy tool which has a built-in feature to test the subdomain takeover vuln. Though, I didn't get lucky by myself, but you can check it out. It has other many good features.***

   - ***Otherwise, you can verify with the help of this repo: <https://github.com/EdOverflow/can-i-take-over-xyz>.***

<br>

 - Your methodology to approach IDOR/prvilege escalation/business logic/information disclosure bugs? Tools you use in your daily recon process?

   - ***If a target has multiple user roles, then I simply login to their respective accounts using "Firefox Multi-Account Containers" plugin and then configure "Autorize" plugin in Burp Suite with low level user's cookies. Then simply by browsing high level user's dashboard I look for any unauthorized access of functionalities.***

   - ***On the other hand, I try to replace the uuid of one user with another to test if sessions are validating properly or not. But be mindful if you approach this way and found an unauthorized access, then you also have to find a way through which you can leak that uuid as well otherwise a triager can also reject this report by saying that uuid is pretty long and falls under enumeration category. So, you might not get any bounty in return (Based on real life experience).***

   - ***Tools which I use in my daily recon process:***

     - ***Sudomy (For Subdomain enumeration and unique parameters list)***

     - ***Burp Suite (For everything)***

     - ***Fuff (Sometimes for real Fuzzing)***

     - ***Arjun (For hidden parameters)***

     - ***My own one-liners for data filtration***

<br>

 - Q1) How do you learn in beginner process and how you avoided procastinating?

 - Q2) Whats your favourite bug you look for and how can one find them?

 - Q3) Last but not the least, if a beginner wants to start, which bug you would recommend for stating journey?

   1. ***I learn only from Google, YouTube, and all the FREE public resources/articles easily available online. And procrastination is one of those things I am still trying to overcome in life while juggling between my studies and bug hunting. Because I don't wanna neglect either of them. That's why I use to set my goals as per the situations and then try to just follow them as much as I can.***

   2. ***I usually like XSS, IDORS, SQL injection bugs and I think one can only become a master in any type of bug through their experience and how many times you have discovered them.***

   3. ***Try IDOR and XSS.***

<br>

 - When I choose a Target I didn't find all its functionalities and then I choose another program and I entered in while loop and this makes me didn't find any bugs. What should I do to overcome this?

   - ***To be honest, this behavior is completely normal when you have just started out or unable to build your own methodology over the time. Plus, this also depends on which type of systems and languages you are most interested in.***

   - ***For instance, I like Linux environments and PHP language and for me this combo is an ideal choice for payloads, but the Fun or Sad part is as a pentester you do not get much choice because any system can be vulnerable and you have to test out all the functionalities it contains.***

   - ***So, I would only suggest you to build your own methodology and decide which type of bugs do you like the most then try to become a master in it or you can also become Jack of all trades and master of none. The choice is up to you, but, what matters the most is your determination and passion for your work which will make you persistent.***

<br>

 - Q1) Your Top 5 Tools that you are using right now?

 - Q2) What are your Top 5 favourite bugs?

   1. ***Top 5 Tools that I am using:***

      - ***Sudomy***

      - ***Burp Suite***

      - ***Dalfox or kxss with xsshunter combo (For XSS findings)***

      - ***SQLmap***

      - ***My eyes and brain :)***

   2. ***My Top 5 favourite bugs are:***

      - ***IDORS / Privilege escalations***

      - ***SSRF***

      - ***XSS / Content injection***

      - ***CSRF***

      - ***SQL injection***

<br>

 - What is your recon methodology? How do you approach for admin panel? Any tips for time management?

   - ***My RECON process does not contain so many things right now, just the basic enumeration process which I have already shared. But, I wanna focus more on JS files and Api key/credentials leaks using Github and other cool bugs in the future.***

   - ***By checking if any recent CVE exists, then look for default credentials or common paths of that technology being used which may get me an unauthorized access.***

   - ***I think for me there is a thin line between procrastination and being hard on myself. Like, if I do too much work, then I feel exhausted and If I do not do anything, then sooner or later I start criticizing myself for not doing anything at all. So, I would only suggest you to set small achievable goals daily and then try to follow them regularly.***

<br>

 - Any weird bug you reported which you are proud of?

   - ***The server was converting the contents of image files into Base64 before uploading. So, I encoded an XSS payload and changed the extension from test.png to test.html and managed to gain a stored XSS. But, unfortunately the report got duplicated.***

<br>

#### The original twitter AMA can be found here :- <https://twitter.com/sillydadddy/status/1379014449323909128>
