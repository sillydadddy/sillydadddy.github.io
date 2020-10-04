---
layout: post
title:  "IDOR in my college website"
categories: write-ups
excerpt: "Bugbounty write up on idor im my college  ! "

author:
  name: Sandeep Krishna
  twitter: MadMaxx
  picture: images/Madmaxx.jpeg
  links:
    - title: Twitter
      url: https://twitter.com/0xCCFFF
      icon: fab fa-twitter-square
  
  
--- 


## IDOR in my college website

My college has a student portal for it’s students to check their semester grades and performance. But it also contains personal information of each student enrolled. So I logged in to my own account and just checked what all I had given there. The URL looked like [https://xyz.com/path3/showmenu.htm](https://target.com/IIT_ERP3/showmenu.htm)

I had the devtools opened for some other purpose and was under the network tab. I observed some POST request being made to an endpoint. This made me wonder… Why it is making POST requests?? I was expecting only a few GET requests as I thought that our institute had our data and it just needs to GET them. But weirdly, it was making POST request too along with other GET requests. The POST request looked something like this ::

![The POST request](https://cdn-images-1.medium.com/max/2000/1*xihrmJkQ2qq8qWpX_WNwYA.jpeg)

I saw the parameter “rollno” where my roll number was given. I just tried changing it to another roll number I know (that of my friend) and I sent the request. Surprisingly it returned all the personal details of my friend.

I was happy to find this bug. I reported it to my college authorities and they immediately fixed it. :)

