---
layout: post
title:  "Infosec Bugbounty AMA with Michele Romano"
categories: infosec-bugbounty-ama
excerpt: " AMA with Michele Romano "
---
# AMA with [Michele Romano](https://twitter.com/Mik317_)

<br>

 - Your favorite bug?

   - ***Client-side: XSSI (I'm recently loving also XSS through message handler)***

   - ***Server-side: Command Injection***

<br>

 - What s your h1 handle ? :)

   - ***Lol, Mik317***

<br>

 - any tip for beginner's starting in bug bounty?

   - ***Have a look to basics and start reading every writeup and guide you can ... Google is full of these amazing and free resources***

<br>

 - 17 and rocking, How do you see yourself in next 5 years? What are your future plans? 
How do you take care of your mental health? When did you start hacking? Favourite bug of all time and story behind it?

   - ***Sincerely I'm still uncertain on future ... I'd like to enter in the research field but also doing BB, but also being employed by a big company ... time will let me know :).***

   - ***Regarding mental health, I tend not to focus too much on bounties and issues, and if I need long breaks I do it and stop. Also, having a different lifestyle makes easier and relaxing doing things.***

   - ***I think it's important also doing gym or having another hobby since that makes you able to refresh your mind and do some exercise (especially for us who're everyday in front of PC)***

   - ***Latins used to say "mens sana in corpore sano" ... a person is performant when mind and body are trained and exercised, not only to do something, but also to avoid doing something else***

<br>

 - what motivates when you get duplicates..

    - ***Duplicate means I was on the right road but someone else had already reported the issue, so I reached my goal (challenge myself). Mostly I don't mind too much if I get a duplicate (but I would prefer anyway to be the first one to report a issue of course) and try to find issues -> which can be chained to the one I got duplicate of so I can get anyway a bonus/valid report :)***

<br>

 - When do you started your Bugbounty journey?
In the beginning of your journey what motivated you the most to become successful hunter?

   - ***I was interested in programming since I wanted to become a game developer. I started frequenting a Italian forum and I happened to check the Infosec category by chance ... I feel in love immediately*** 😂 ***(now it's almost 4/5 years ago).***

   - ***Regarding motivation, I always liked challenging my-self and others ... and that's the most competitive field I could find. Money haven't ever been the most important factor, even if I admit it's something which made me persevere ;)***

     - Cool!  And have you played any ctfs or labs in the beginning or u directly dived into  hunting real applications?

       - ***I didn't like very much CTFs even if I think they're a really good way to learn new things. I did some practice with vulnerable labs like DVWA and some Google Gruyere exercises, then I just tried on real websites.***

<br>

 - How did you manage studies (like schooling works) and hacking (how many hours per day)?

   - ***That's still one of the harder things I have to do:***

     - ***BB is my hobby while school, gym and work are my life, so I try to balance them all basing also on schedules I've for different activities. In general I hunt every day 0/1/2 hour when I come back from school and 1/2 in the night***

   - ***That depends mostly by the period:*** 
   
     - ***if I have tests/exams there are days I don't turn on the PC for more than 30 mins.***
    
     - ***Same if I need to prepare for an experience like Uni courses and other.***

     - ***In the weekend instead I hunt 3/4 hours per day***

<br>

 - What educational hacking resources do you wish existed that doesn't exist today?

   - ***Surely IDK: writeups are the most important resource where you can learn along with presentations made in security events.***

 <br>

 - How much time did you give to learn before starting bb? Did you planned to complete some course/content and then start bb?

   - ***I think it took ~6/7 months because I registered on H1 on Jan 2018, but my first bug was reported on Aug 2018.***

   - ***In that time I looked at every possible writeup I could understand and studied a bit of programming and manuals like "Web Hacking 101". The rest is experience ;***

 <br>
 
 - From where did you learn? If given a chance to go back in time, what will do more and what would you do less?

   - ***Actually I started from an Italian infosec forum and then started studying from manuals and ebooks + courses (ig I'm not wrong I discussed this in https://huntr.dev/blog/ep-001-bug-huntr-mik-317) :)***

   - ***If I could go back in time I would change my approach: there was a time I was more interested in being right than understanding actually why I wasn't lool. In this case philosophy helped me to understand why I wasn't and why I shouldn't***

 <br>
 
  - best tools u use??
 
    - ***Apart BurpSuite, SQLmap and arjun***

      - is arjun good?
        
        - ***Yeah, I tested with it some of the endpoints I found "useless" and sometimes the tool retrieved good parameters which (in some occasions) lead to XSS or other issues :)***

 <br>

 - What tools you use and have you made your own, also in which lang?😁

   - ***I mostly use BurpSuite, SQLmap (without no luck mostly), arjun, nmap, dirsearch and gitrob. Yeah, I automated my recon with a tool I wrote in Py and other minor tools to generate CSRF forms or find malicious JS snippets. If the tools have to be powerful I use Py, if not JS***

 <br>

 - I use burp community ,for my bug hunting , how burp pro can help me find more bugs ? did you used burp scanner to find a bugs ?

    - ***Actually I'm using Burp Pro since 2 months, while until now I used the community ed. I found it comfortable and full of plugins I didn't have access to, but in general I haven't yet found issues ONLY using Burp. The \`content\` check and other functionalities however are good to find useful endpoints or paths with secret information. Someone said \`collaborator\` is also a great tool, but before having this one I used everywhere \`ngrok\` + \`dns/http server\` and it worked anyway.***

    - ***That said, I'm still exploring it, so maybe there are 5000 functionalities which will be useful :)***

 <br>
 
 - What are the burp plugins you use?

   - ***A lot: XML2JSON, Param Miner, Turbo Intruder, Brida, Paramalyzer, Deserialization Scanner, Reflection, CSRF***

 <br>

 - What was your biggest bounty till now?
 Elaborate about your bugbounty setup(e.g. toolset, checklist, note keeping, vps etc)

   1. ***2k\*2 (actually was a chain of 3 different bugs which led me to the total amount) - yeah, I know it's quite unfair but I worked mostly on VDPs lool***

   2. ***I made a good description on my setup on https://huntr.dev/blog/ep-001-bug-huntr-mik-317*** 😊 ***Regarding note keeping, I limit myself to insert in a -> textual file the most important endpoints and information + eventual things which could be useful if I fund bug X (for example: self-XSS in page /XXX: if I found CSRF I can achieve stored-XSS without interaction on victim's account :)) - it's all about leveraging what you find***

 <br>
 
 - Any tips for beginners in android hacking ?
 
   - ***I've started this year doing a bit of android hacking, and I found very useful reading writeups regarding issues found on Twitter/Insta/Facebook and also "The mobile Application Hacker's Handbook" guide, which is a good starting point. Also H1 videos like https://www.youtube.com/watch?v=y0O3sCX9ftM***

 <br>

 - what you suggest about , android hacking like should i use hardware or virtual , what you prefer ?

   - ***I'm using a simple Android emulator (the one of Android studio), but I think I'm gonna buy a smartphone for tests really soon.***

<br>

  - any tips for finding server side bugs

    - ***That's really general, but I try to find all the functionalities which interact with the server and then try to get errors/strange behaviors to understand how the application works. Basically, if I have a website which parses photo I try thinking what are the action made by the server. For example, if the image is retrieved remotely, I try SSRF; If image is converted I check for errors when filenames with bash syntax and characters are supplied; if a SVG is parsed I try XXE; It's basically trying all the possibilities until you find something "strange"***

 <br>

 - Any tips regarding CMD INJECTION bugs ? 
Vulnerable fields ?

   - ***I tend to understand the web app logic and then ask myself "will this input be processed using a shell command? if so how?".***

   - ***The other strategy I use is fuzzing for some \`bash syntax\` characters, in order to find eventual errors/behaviors which could lead me to understand how is the input processed.***

   - ***Regarding fields, you can find it mostly in actions which manipulate images and eventually filenames, but sometimes it's completely strange, like in password field, so the key is fuzzing and see what are the different responses***

 <br>

 - How to focus on trying to find Server side bugs?

   - ***It's important focusing on the logic of the application and all the possible stages which require server actions. I generally don't focus on client or server side, but I give a look to everything and then try to find bugs, which makes me motivated enough to hunt on both of 'em***

     - Where to look for those apart from the obvious uploads and parameters?

       - ***That's based on the first answer: understanding how your input is processed is important. I generally try to put malformed inputs to see if I get errors/strange responses which could help me understanding how my input is concatenated in a command or parsed in specific ways***

 <br>
 
 - Your approch to hunt authentication related bug ex Auth2.0

   - ***Sincerely I haven't yet hunted really much for this type of bugs, so what I know is few attacks. Principally I check for \`open redirects\` on those auth methods and I try to reproduce on my target some attacks I already saw on H1 reports disclosed or in some resources like:***

     - ***https://www.bugcrowd.com/resources/webinars/hacking-oauth2-0-for-fun-and-profit/#accept***

     - ***https://medium.com/a-bugz-life/the-wondeful-world-of-oauth-bug-bounty-edition-af3073b354c1***

     - ***https://medium.com/@pravinponnusamy/oauth-related-vulnerabilities-ac2e2904f152***

     - ***https://gauravnarwani.com/oauth-2-0-security/***

 <br>

 - What is the most common place you check for xss payload?

   - ***Search field and contact pages, or in some cases \`comment\` sections. But in my case \`search\` fields are 90% times vulnerable (many people check only reflected and not DOM ... check the JS too ;))***

 <br>

 - What is the next step you do if you get some hidden parameters using arjun? What kind of attacks you try

   - ***It depends mostly on the functionality of the endpoint where they're discovered, but in general I check them for open redirect/XSS and SSRF/command injection. It happened also I could find a XXE indirectly using it, but it depends mostly on the meaning the parameter assumes in both client and server side.***

     - Like what if the hidden parameters are named randomly like ait, wpt? Then how you try to get about the parameter

       - ***90% times I check if:***

         - ***are reflected in headers/HTML in specific locations which give me context about what they are used for***

         - ***accept only specific type of values (does it accept only integers? what could it represent)***

         - ***try to give 'em strange values and see if backend retrieves errors/debug info or just comments in the HTML (when pages are made in dynamic ways)***

         - ***they show something different when I change a valid value (if the valid value is given)***

         - ***search on Google for websites with the same parameter and try to understand what's his function***

 <br>

 - When I see a XmlHttpRequest in the Burp History is there anyway to find the js code it called it

   - ***IDK if it's possible using Burp (never did it), but probably you can use a plugin for it like Linkfinder which identifies the endpoints called and the file + line where the string occurs***

<br>

 - Which types of bugs did you find on Sony vdp?

   - ***Actually HTML inj (WAF were very good and I didn't lost much time trying to bypass 'em) and CSRF ;)***

 <br>

 - How important is automation?

   - ***I automate things only during recon to get some infos and bruteforce paths/parameters. The rest is manual analysis :)***

 <br>
 
 - Do you do any kind of automation that runs frequently  for  getting the deltas (new subdomain, change in a website etc etc) ? Getting alerts on code push , new subdomains ,etc

   - ***Sincerely not. I tend to automate only the recon stage the first time I look at my target, then I have some manual checks every X weeks. I feel however I should start creating something which makes me able to monitor changes in big scopes :)***

 <br>

 - What about fuzzing and fuzzing automation , notification too .

   - ***I tend to fuzz specific fields to see the different responses I can get and eventually the new info regarding debug traces etc ..., but I don't automate recursively.***

   - ***Notifications? I never used them since when I'm in front of the PC I'm 99% seeing everything, if I'm not I'm busy***

 <br>

  - Custom Wordlists always?

    - ***Never used custom wordlists except for bruteforcing paths on specific servers (like, if server is using Apache ofc I use apache wordlist)***
 
 <br>

 - Your response when you're asked to hack yo friend's ex's Insta?

    - ***Fortunately it happened only twice (I'm good in keeping secret my 2' life), and I answered something like "How can I win the heart of your ex if I hack her?"*** 😂

