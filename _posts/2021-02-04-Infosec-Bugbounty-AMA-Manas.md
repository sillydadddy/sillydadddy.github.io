---
layout: post
title:  "Infosec Bugbounty AMA with Manas"
categories: infosec-bugbounty-ama
excerpt : "AMA with Manas"
author: Gurvinder Singh
---

# AMA with [Manas](https://twitter.com/ManasH4rsh)

<br>

 - Methods for SSRF?

   - ***Well, it differs person to person and my favorites are scrapping endpoints from GAU and looking for default params.***

<br>

 - What have you automated uptill now?

   - ***A lot of things... I have combined the tools I use... I dont use VPS these days so I have my own oneliners. I keep making them because it makes the task easy and there are many things on the way.***

<br>

 - How long it took to find your first bug? How long you've been doing bug bounties?

   - ***It took me 6-7 days. I was lucky I got an IDOR but it might not be the case for everyone. You need to keep going and enjoy the process. Its been 9 months since I started.***

<br>

 - Tips for IDOR and SSRF?

   - ***Check every parameter and endpoint....keep an eye of every number which you are seeing in parameters/url. It goes for files as well. You might find an IDOR. For SSRF, default parameters i.e ?url=, ?redir= can be good to look for. Use burp search a lot with keywords.***

<br>

 - I am confused between so many fields inside security, like what to go for first. Sometimes it is cloud security, sometimes it's some or other. Couldn't fix my mind to any one or say stick to one. Any tips?

   - ***It is totally up to you what are you good at. If you will ask to me I will tell you appsec, if you will ask a cloud security engineer he will refer you to his field. So, take your time, don't force yourself to be in a race. Try everything which comes in way.***

<br>

 - How to approach target? Which tools you use daily recon process? Tips for IDOR and business logic bugs?

   - ***When it comes to approach it should be like you really need to dig deeper since a lot of people are doing the same thing with automating stuff. Keep in mind automation works only as a reference and you'll have to check the functionality of a website on their main app.***

   - ***I normally use amass, aquatone, dirsearch/ffuf, httpx and gau. If the target is huge I sometimes use nuclei. Also, some burp extensions like turbo intruder, authorize and logger++ are good to have.***

   - ***For IDORs, look for every numerical value and try to manipulate it changing with another number...use authorize and for business logics you need to understand the app and think how can you manipulate the customer/org data. There are so many scenarios.***

<br>

 - Can you share tips for hacking JWT?

   - ***Some basic things to check for JWT are if you can change the algorithm to "none" or if you can bruteforce the secret key. Also, Key ID allows directory traversal sometimes and you should always check if it is not sanitized properly.***

<br>

 - Which checklist you follow while hunting for bugs?

   - ***I have created my own mate...and I would highly suggest you to make yours from today onwards. Like see what bugs you can exploit and keep a note of it so that you could apply the same next time.***

<br>

 - Which one do you mainly hunt for, Client-side or Server-side vulnerabilities?
 
   - ***Both.....I mean you don't need to leave anything which you can find.***

<br>

 - How to keep motivated to hunt, as I feel overwhelming most of the time, imposter syndrome hit hard also. Is it me only or a generalized phenomenon in this field? What will be top 5 bugs class you will suggest someone with a intermediate skills to hunt for?

   - ***For your first question this should help: <https://medium.com/bugbountywriteup/pushing-yourself-through-hard-hunting-days-a-bug-hunter-perspective-d03b4c16b04>.***

   - ***Its not about top 5, lets say the bugs you should always look for:***

	   1. ***SSRFs***

	   2. ***Business logics***

	   3. ***XSS***

	   4. ***SQL injections***

	   5. ***Hardcoded credentials in APIs***

<br>

 - Any tips to get job in infosec because in most companies you needs 2-5 year experience?

   - ***I agree but you are not 100% true..some companies do hire freshers and you might get less package but if you wanna start there are some companies who do it..you just need to make enough connections.***

<br>

 - How do you learn something new?

   - ***[@PentesterLab](https://twitter.com/PentesterLab), [@InfoSecComm](https://twitter.com/InfoSecComm), [@PortSwigger](https://twitter.com/PortSwigger) and [@Google](https://twitter.com/Google) as well.***

<br>

 - According to you, how much programming needs in hunting or we hunt without programming also?

   - ***As everyone says programming is not a big deal. For me its like programming gives you an edge over people who don't know it. There ARE exceptions but its always good to have some basics of php, JavaScript and atleast one scripting language.***

<br>

 - How to do automation for recon?

 - How do you approach a target after basic enumeration?

 - How to improve skills?

   - ***It differs from person to person but I think using a VPS and writing your own script would be great.***

   - ***I try to dig deep on the main app since it gives me an idea how the application is behaving. Once I know what the app does, I can go ahead and try my skillset on it.***

   - ***For improving skills, keep learning from other's mistake so that you don't repeat the same. Also, follow good people from community and keep scraping stuff from [@InfoSecComm](https://infosecwriteups.com/), [@PentesterLab](https://pentesterlab.com/), [@PortSwigger](https://portswigger.net/web-security)....read research papers for a particular vulnerability.***

<br>

 - Can you tell how did you get started in bug bounties? i.e. focused on several type of bugs, hunting time, which resources you used etc.

   - ***Yeah I started it since I had a craze for hacking stuff. I literally had no idea how bounty can change my life. I heard it from some people and since I was new everything was fascinating. I learned one bug at a time and moved to next. Luckily I had people who guided me for better.***

   - ***I learn stuff mainly from writeups i.e. [@InfoSecComm](https://infosecwriteups.com/), [@PentesterLand](https://pentesterlab.com/) and googling everything. Also, [@PortSwigger](https://portswigger.net/web-security) has been a great resource.***

<br>

 - Any tips to confirm blind SQLi(time-based)? Automation trick to find SSRF?

   - ***Yeah! Check the response time once you try your payload in the request. You will feel its enough time difference each time you put a time-based sqli payload. Also, as soon as you find a time based SQLi, fire up your SQLmap.***

   - ***For automating SSRF, use collaborator everywhere along with the GAU tool. It will give you default parameters...grep them and fireup your burp with collected URLs.***

<br>

 - If you can go back in time and do that one thing which you initially missed while doing bug hunting what was it?

   - ***Ummm starting bug bounties when I was in college, I would have got plenty of time to learn and earn! You have time though.***

<br>

 - Advice for newcomers who have just started doing bug bounties?

   - ***Don't focus on money in your initial days because it hurts when it doesn't meet your expectations. Focus on learning, make notes of everything which is new for you and ask...ask a lot of questions when you get confused. Someone will answer.***

<br>

 - Path To Become ASE?

   - ***Make connections so that you could apply in good companies...learn all the basics of owasp top 10 and their exploits.***

<br>

 - Tools that you use Most?

   - ***I assume you are asking except burp...It would be a tie between amass and aquatone.***

<br>

 - What have been your biggest achievement while learning and exploring Bug bounty?

   - ***My biggest achievement would be getting some awesome friends who pulled me up where I am today. Money and all are okay but what matters most is how is your circle.***

<br>

 - How you enumerate subdomains of target domain without missing any subdomains, any suggestions...? Tools for subdomains enumeration? How you approach sensitive information disclosed and javascript file?

   - ***I normally use amass along with subfinder and it gives prettt good results. I hardly miss any subdomain. You should always use two tools for discovering assests. Sensitive information are sometthing which come with js files or request/response. Try to find endpoints with GAU.***

   - ***Read js files manually and you might get good things in it like endpoints, urls which redirect somewhere else.***

<br>

 - Suggestions for mobile app and api pentesting?

   - ***For API pentesting, its web app testing only with something integrated with it. Look for common bugs i.e IDORs and SQLi along with Hardcoded creds. For Mobile, solve the [@PentesterLab](https://pentesterlab.com/) android badge for a better understanding since I am learning android too.***

<br>

 - As a beginner, how do I select a program for hunting.. From where do I select like from hackerone, bugcrowd, public program, hackerone invite by CTF?

   - ***As a beginner, platform doesn't matter. What matters most is programs. Choose a program with larger scope and VDPs are very good to start with. Once you get some private invites after earning some points, hack on them and try to find stuff.***

<br>

 - Please share some tips & hunt flow regarding .js recon.

   - ***Awesome! So, for JS recon, first thing you need to keep in mind is manual recon. Try to read the js files with the help of developer tools > network tab. JS files are not only for finding hardcoded creds but also for scrapping hidden endpoints which automation might miss.***

   - ***Also, you can use linkfinder for scrapping URLs which are included in a website. But developer tools are best imo.***

<br>

 - How to not hunt bug's in an application and what are the things you always look for in a target before starting to hunting on a target?

   - ***I normally look for the scope and the functionality within an app..also, how are their subdomains? Are they holding something new? These are the things..also can we create multile user and check them? More functionality, more bugs!***

<br>

 - Any place or method to master Oauth 2.0 bugs like A to Z?

   - ***For Oauth there are pretty good labs on [@PortSwigger](https://portswigger.net/web-security). I have learnt them recently and I must say those are awesome to get a hands-on. For some more stuff, you can subscribe to [@PentesterLab](pentesterlab.com/) as well.***

<br>

 - I just wanna ask you I almost hit 11 months in bug bounty hunting field without finding any valid bug, I just wanna ask you how to stick hunting on single program I can't do it I don't know why I didn't find a program I am comfortable with!?

   - ***Mate its tough to get going but you have no other option. You cant simply give up because after some years you will think you were not enough strong to fight back and you will feel bad. Stick with a program which you are friendly with for example Facebook.***

<br>

 - Which book you would recommend for beginners?

   - ***Web app hackers handbook for sure...and tangled web. OWASP testing guide is also very handy.***

<br>

 - How do you balance learning and hacking?

   - ***I keep a note of things which I need to do in a day...like sometimes I hack on weekdays after my work. Sometimes i take all weekend hours to hunt. You need to calculate what things you can do in the time you have except your job and its easy after that.***

<br>

 - Learning or Hacking or Both simultaneously?

   - ***Learning is a process mate! Whatever you do learning walks together. Same goes for hacking as well. You need to stay practical always.***

<br>

 - What VPS do you recommend for doing bug bounty?

   - ***I think Google VPS would be the best...I am loving it.***

<br>

 - Any weird bug you reported that you are proud of?

   - ***Admin/admin.***
