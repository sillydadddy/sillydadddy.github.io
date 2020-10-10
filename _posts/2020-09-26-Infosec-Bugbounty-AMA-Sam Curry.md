---
layout: post
title:  "Infosec Bugbounty AMA with Sam Curry"
categories: infosec-bugbounty-ama
---
# AMA with [Sam Curry](https://twitter.com/samwcyo)

<br>

- How u got into hacking ? What are the bugs you advice for me to look for ? and What are your fav. tools exp. Burp. If u wanna give an Advice to newbie bughunter whats that ?? (it should be unique) Btw Thanks 😍

   - ***Hey! - I got into hacking from the video game community. - Favorite bugs to look for are directory traversal and SSRF. - Favorite tool besides Burp is SQLmap - Start hacking as soon as possible Cheers***

 - Hey ! , I'm a Begginner and couldn't decide to choose either between Public Or Private programs, are Private programa more vulnerable or public programs more secure? Thanks in advance! And you are Amazing (as always :)
 
   - ***There really isn't a "more vulnerable" - if a program is public, they're likely more mature and are tested to be under public eye, whilst private programs may be more young/have specific expectations of the researchers. This does not really mean much for the actual codebase.***

- while learning about bugs what mistakes you made and what methodology you suggest to learn a bug 》Did Recon is neccessary to learn especially for beginners..? 》what is methodology while a hunting bugs..?

   - ***I made the mistake initially of depending on other people for things I could've learned myself and ended up digging myself into a hole when I went back to figure it out. Recon is not necessary but if you enjoy it then go for it. See other replies re: methodology :)***

- Whats your interesting findings yet? Where you will see in the 5 years? Any goal?

  - ***I have a few things that I've blogged about @ https://samcurry.net/ and plan to blog about moving forward. Have found a few neat zero days and CVEs that I hope to be able to talk about soon. No real 5 year goals. Just want to be doing interesting and helpful work.***
  
- we come to a situation which is kind of deadlock and we are stuck at one place. We cannot find any interesting bugs. What do you suggest to cope up with this?

  - ***Hard situation. In my experience, while under time constraints, I can never focus on anything. I've fixed this by trying to forget about the situation and just pay attention to what I'm hacking. Once you get one good bug (the hard part) they seem to flow easier.***
  
- There are so many cases we should test in an Web App. How do you make sure that you are testing each of these cases?
  - ***To be honest, the only limitation here is time. You're never going to get to test everything, everywhere, and if you do then it'll become too confusing too fast. The trick people use to find bugs is understanding what bugs to test for and where. People who hack on Facebook will tell you that it's often not worth the time to test for standard bugs (XSS, SQLi, etc.) because they've built their system in a way where it's much harder. They instead look for logic bugs and access control issues that seem to be much more common***
  
- 
