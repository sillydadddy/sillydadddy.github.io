---
layout: post
title:  "Infosec Bugbounty AMA with Abdillah Hasny"
categories: infosec-bugbounty-ama
excerpt : "AMA with Abdillah Hasny"
author: Gurvinder Singh
---

# AMA with [Abdillah Hasny](https://twitter.com/abdilahrf)

<br>

 - How did you get involved with information security?

   - ***My journey with hacking started from my interested in playing video games at ages of 12, while playing games I always wondering the people that using cheat to play the game and i was about thinking it will be cool if i also can create cheat my self since then***

   - ***I was learning reading memory and stuff to hack a game and create cheat. long story short i school software engineering but while school i actually give more attention to the security aspect rather than the development.***

   - ***Thats how i could break application betterwhen i understand how to build the apps.***

<br>

 - What is your hunting methodology? Recon process? Which is your niche bug (which type of bug you hunt most and focus on)? Any notes you can share?

   - ***- Subdomain Enumeration (subfinder/assetfinder/chaos/amass)***

   - ***- WayBack Machine (gau)***

   - ***- Directory Enumeration (ffuf)***

   - ***- Screenshot (pageres)***

   - ***- CVE Scan (nuclei & jaeles)***

   - ***Other than that just recon based on the application functionality.***

   - ***I don't have niche bug category but i was more into Server Side Bugs rather than client side.***

   - ***I've try to put my note in this repository, just like everyone who try to put their note there so everyone could learn and have an idea what and how to test: <https://github.com/KathanP19/HowToHunt>.***

<br>

 - Q1) How did you managed your time at beginning?

 - Q2) How was your setup back than and now?

 - Q3) Don’t you have neck pain, if yes than you solved that problem? 

 - Q4) Any advice for beginner?

    1. ***I didn't have any time management at the beginning but now i still trying to get better at manage my time for bugbounty its really important to have the time management because if you can't control yourself when to stop you can just hunting without stop and it was not good for your health and the efficiency to finding bug also give you high risk to get a burnout.***

	2. ***Nothing much setup back then, just a windows 7 and mobaxterm. but now my go to is using windows 10 + WSL V2 is perfectly fit for any cases.***

	3. ***I've rarely have neck pain but if you have you could try <https://youtube.com/watch?v=z91Ef5DH9QY> I have been trying this and its working to remove the pain.***

	4. ***Nowadays beginner need to be carefull while finding a resource to learn, because now everyone is sharing a thing but there is a thing that could lead you to be better hacker and there is also thing that could misslead your understanding. I could suggest the best resource for beginner : <https://portswigger.net/web-security/all-labs> and playing HackThebox.***

<br>

 - What note taking app is your goto when you are bughunting and why?

   - ***My note taking app is <https://joplinapp.org>. The reason is because the app support markdown and also have quite usefull WSIWYG. also the apps is Open Source and you could sync all your note to any of your device flawlessly.***

<br>

 - How do you know what depth you need to learn to know about a specific topic? I mean how do you figure out that OK, this much of info will be okay for me right now, I'll learn when I need it later?

   - ***Lets take an example, if i want to learn about smuggling I try to read the practical example of the exploitation and the key note that i need to understand is how to detect the vuln, we can learn how to exploit it later when we have the vuln at the first place.***

   - ***But on the other case, if you wanted to automate the thing you need to build a reliable exploit by trying out your exploit in a vulnerable system that you can found in CTF Challenges or Any Labs that provide vulnerable machine related to the topic.***

   - ***"Smuggling" that I mean was HTTP Request smuggling.***

<br>

 - I'm overwhelmed by resources- I have just started in bug bounty - and I do download any book related to the field .. how to get myself organized?

   - ***You need to focus to learn one topic at a time until you feel understand the whole, and try to implement what you learn in bugbounty program.***

   - ***Don't rush to learn, don't look other people success and comparing with yourself, it will bad for your mental health. so just focusing on your self and appreciate what you do and learn each day.***

   - ***Don't try to get all resources into your reading list, just pick 1-2 reading a day, create your personal note to track your progress and what you plan for the next day so you can evaluate and see the progess time by time.***

<br>

 - How one should learn manual exploitation rather than using tools?

   - ***Learning exploitation manually is better than blindly using tools and trusting the output of tools, because not all the vulnerability could be found by tools, and most of the time you need to process the finding from tools to make an security impact.***

   - ***I would highly recommend to understand how the tools work and start to do it manually, use tools to get your job faster it is okay if you understand the things going behind it.***
