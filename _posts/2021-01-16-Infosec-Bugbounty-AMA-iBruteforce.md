---
layout: post
title:  "Infosec Bugbounty AMA with iBruteforce"
categories: infosec-bugbounty-ama
excerpt : "AMA with iBruteforce"
author: Gurvinder Singh
---

# AMA with [iBruteforce](https://twitter.com/iBruteSec)

<br>

 - Can you suggest some non technical bug?  Other than idor and subdomain takeover. So that I can learn it and hunt on all programs.

   - ***By non technical bug - I guess you mean bug classes that are easy to understand? I’d say CSRF is pretty easy to hunt for. All you’ve to do is simply check if the sensitive function of the application is protected by CSRF tokens. If it does, see if you can bypass it.***

<br>

 - Which bug types to approach in increasing level of difficulty?

   - ***I’d then say CSRF, Open Redirect, XSS are pretty easy to learn. Exploiting XSS can be hard if you’re faced with filters/WAF but you can practice beating them via challenges. Check out [@BugBountyHunt3r](https://twitter.com/BugBountyHunt3r) and [@WebSecAcademy](https://twitter.com/WebSecAcademy). They’ve got some great content and hands on lab!***

<br>

 - Please tell me everything about your content discovery method. How do you find hidden endpoints and parameters? How do you create your custom wordlist? Any checklist for broken access control?

   - ***I don’t really do a lot of directory bruteforcing, if I do I’ll run it against a wordlist that I’ve created specific to the target with seclist added in.***

   - ***Mainly javascript flies and waybackmachine. I’d look through most of the robots files to see what they’re in there.***
