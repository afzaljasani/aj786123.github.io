---
layout: post
title: Installing Google Analytics on Jekyll Site
comments: true
description: 
category: blog
---

A few weeks ago I finally decided to install Google Analytics on my personal website. The reason behind installing GA was to get a better understanding of how large of an audience was coming to my website and how they were interacting with each article. GA is great if you know how to navigate through all of its features and pull insights from the various metrics they track. I will admit though, if I had not learned how to use GA from previous internships or my current work experience, it would be a bit overwhelming. GA is robust and offers many tutorials through Google to become an analytics master, but sometimes that's not enough.

Installing GA tracking code was actually pretty straightforward. I first went to the Google Analytics page to set up my account and get the tracking code. This is the screen to access your account and get the tracking code. 

![My helpful screenshot](/assets/GA_homescreen.png)

![Screenshot](/assets/GA_admin.png)

![My second helpful screenshot](/assets/GA_trackingcode.png)

After you find your tracking code, you need to navigate inside your folers to the _includes folder. In this folder you should open up the head.html file. Inside the head.html file you will want to paste the tracking code in between the "</head>" tag. 

![texteditor](/assets/GA_texteditor.png)

That's all there is to it! You know have Google Analytics tracking enabled for your Jekyll site. Happy data tracking :) 




