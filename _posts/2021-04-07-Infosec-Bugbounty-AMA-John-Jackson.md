---
layout: post
title:  "Infosec Bugbounty AMA with John Jackson"
categories: infosec-bugbounty-ama
excerpt : "AMA with John Jackson"
author: Gurvinder Singh
---

# AMA with [John Jackson](https://twitter.com/johnjhacking)

<br>

## Senior AppSec Engineer [@Shutterstock](https://twitter.com/Shutterstock) 🔥, Founder of [@sakurasamuraii](https://twitter.com/sakurasamuraii) 💥, Author of Corporate Cybersecurity [@WileyGlobal](https://twitter.com/johnjhacking) 📘

<br>

 - Q1) Favorite bug you found?

 - Q2) What bug took you time to execute/escalate?

 - Q3) Favourite tools and plugins?

 - Q4) What is that one book you would suggest everyone should read(infosec and non)?

 - Q5) What will be your msg for your younger self starting his journey?

 - Q6) Proud purchase/meme?

   1. ***git-credentials exposed on the client side, led to breaching the United Nations.***

   2. ***Probably anything related to taking an RFI/LFI to account takeover or remote code exec.***

   3. ***Dirsearch, Nuclei, Nmapautomator, Dalfox, Burpsuite, Aquatone.***

   4. ***The Web Application Hacker's Handbook // The Alchemist.***

   5. ***Stop caring about what others think and to just...go for it.***

   6. ***Proud purchase: Every book i've ever bought // I'm proud of my securety stonks template: <https://www.reddit.com/r/MemeTemplatesOfficial/comments/ke348g/stonks_meme_cybersecurity_variant_securety/>.***

<br>

 - What is your hunting methodology? Which is your niche bug (which type of bug you hunt most and focus on)? Any notes you can share?

   - ***My methodology while hacking is to think like an APT. I don't usually touch XSS or anything that's too mild. I try to focus on looking for CVEs or known-attack vectors: out of date applications, etc. I like RCE bugs particularly.***

   - ***Best note I can give you is to take notes. Focus on annotating vectors that are of interest and cutting out any that aren't progressing. Having an idea of possible vulns is the only way you're going to hack the asset. Run through the phases of hacking.***

<br>

 - I hear you know about netMask?

   - ***Sure do! The whole debacle actually stemmed from research that I had originally conducted on npm private-ip. A researcher was able to bypass SSRF multiple times, and after investigating with a co-worker [Harold Hunt] we found the private-ip package using bad regex.***

   - ***The regex didn't account for any localhost variations at all, so using something like http://127.0.0.1 would be an adequate payload to bypass the regex rules to prevent SSRF. Additional conversions such as http://0000.0000.0000.0000 worked as well.***

   - ***Fast forward a few months after resolving that CVE, [@Koroeskohr](https://twitter.com/Koroeskohr) comes along with an octal bypass and stated that it worked on another package using similar logic. He showed me that octal translations, even if private, were read as public. He noted this on npm netmask.***

   - ***I immediately knew that it was going to cause heaps of problems and was yet another CVE, but didn't realize how big it was until I brought in [@sickcodes](https://twitter.com/sickcodes), [@tensor_bodega](https://twitter.com/tensor_bodega), [@kaoudis](https://twitter.com/kaoudis) for Software engineering assistance.***

   - ***What do these peeps start doing? Of course, escalating it further and further. The true impact assessment is nowhere near done. It affects "a lot" and is legitimately a revolutionary vulnerability for the Networking/IPv4 space. Tons of IP blocking logic can be bypassed.***

   - ***In fact, I even managed to pickup a quick bounty for the CVE immediately. I found a vulnerability in Brave in which netmask was being used as IP logic blocking against their BAT Ledger servers. I proved that I could use the private ip octal conversion to bypass ACLs and DDoS.***

   - ***The TL;DR: Octal is dead. No applications should be processing octal.***

<br>

 - Do you test for blind SSRF/LFI? What tools you use in your automation? How you bypassing server-side filtering while file upload vulnerability?

   - ***I test for anything that I possibly can. SSRF/LFI are hard to automate in my experience, but you can use [@0xAsm0d3us](https://twitter.com/0xAsm0d3us)'s Paramspider tool to look for possible SSRF occurrences and then test further. LFISuite is good if you have a known LFI vector.***

   - ***For bypassing filters my first shot is double extensions. You'd be surprised to see just how many applications use logic that doesn't do a good job of preventing this.***

<br>

 - If you have triage experience, then please share that which types of vulnerability are being reported nowadays and what are the characteristics of an ideal bug bounty report?

   - ***I'm not a triager, I'm an AppSec eng so I can't speak for the bug bounty field. However, I would say that I see a lot of XSS bugs - they are extremely common. Ideal report is one that flows like this:***

   - ***Summary -> Steps to replicate -> Impact -> Additional considerations.***

<br>

 - As a triager, what makes a report looks interesting from the first few lines?

   - ***I'm not a triager, so I can't exactly speak on their behalf [I receive the reports from the triagers] -- However, I can tell you that I take particular interest in reports that move from client-side to server side or involve flawed business logic.***

<br>

 - How you think about memes? Any secret tips?

   - ***I just think about funny occurrences or frustrations that I've either seen or experienced and then let them flow into meme format.***
