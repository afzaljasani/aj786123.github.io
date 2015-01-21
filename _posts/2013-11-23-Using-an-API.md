---
layout: post
title: Using an API for the First Time
comments: true
description: api, github, flowdock, gif, python
category: blog
---

This past summer as I continued my internship with Parse.ly I got the opportunity to work on a side project that did not involve business or marketing, but instead programming. Everyone at Parse.ly loved the idea of me going out of my way to learn something and program it. This small project came up one day when we were using our IRC client, Flowdock, and the CEO asking if we could somehow write commands into Flowdock which would then return GIFs of the specific keywords we included. As any other tech startup we love using GIFs :) For example anyone in any of the flows(chats) could put “!catgif” and Flowdock would return a random GIF of a cat! Sounds pretty awesome right? Well the really awesome part is that Flowdock actually has an API that users can interact with and create such a program. Having only minimal python skills and a little help from a fellow intern I got started on the project. The specific API which I used for this project was the streaming API and the push API. I also needed to find a resource where I could pull random GIFs, for this I used <http://thecatapi.com/&#8221>.

What I needed to do first was lay out a few functions which would take in the information I needed and leave the rest out. Using the stream API enabled me to process all the information that went into each flow and find specific keywords that matched what I wanted to use as a command. After finding the specific keywords and if they matched the next function would send a GIF back through flowdock in that specific flow where the keyword was found. I was able to change who appeared to return the GIF as well. As a default I put it as Flowbot because it was our very own robot which interacted with us. Later on people used the code to change it to other people’s name and do funny things with it.

Overall, using the Flowdock API was an interesting and enriching experience. I think it was a good API to use as a beginner programmer and Flowdock themselves provided plenty of documentation to help me along the way. As I practice and learn more python I hope to user other APIs to build different programs.

You can find the code here on github: <https://github.com/aj786123/pyFlowBot/blob/master/pyflowbot.py>