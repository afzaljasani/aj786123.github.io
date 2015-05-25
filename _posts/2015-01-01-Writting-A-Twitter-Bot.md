---
layout: post
title: Writing a Twitter Bot 
comments: true
description: twitter bot, python, web scraping, lyrics, philosopher
category: blog
---

I recently completed a fun python project which involved creating a twitter bot. The idea came from one of my cowokers who had previously written a twitter bot for fun. He suggested it as project for me to learn more about python and a few different libaries available. I decided it would be funny to scrape lyrics from azlyrics.com and assign them to a famous philosopher. It would look as if the rap lyric line was a quote from them and hopefully cause a few laughs. 

The first time I wrote the program I tried using a lyrics API website called LyricWikia API. After realizing it only returned lyrics in a psuedo-JSON format, I ran into several other problems with escape erros. Going back to what my friend originally suggested with web scraping, I decided to used azlyrics.com for its simplicity in HTML format. I also decided to use Twython, the python wrapper for the Twitter API.

Urllib2 and Requests were libraries I originally had no experience with either but soon learned how powerful they were. Getting to pages and pulling the HTML was really interesting as well. 

I organized my program in the following order:

1. Pick a random artist from a list that I specified. Currently Nas, Jay-Z and T.I. are being used which should provide plenty of lines.

2. Form the URL of the selected artist's page. This was used in order to pull up the page with all the artist's songs ever written. 
3. Pick a random song from the list. 

4. Pull the lyrics from from the song page using xpath. Plae each line into a list and randomly choose a line from that list.

5. Clean up the lyrics to strip away any escape errors. 

6. Assign a random philosopher from a list I specified. 

7. Tweet it! 

Breaking up the program into these steps made it more clear to me what was needed to get the twitter bot running. Overall, the documentation online and various tutorials that are available make this a fun and relatively easy project to accomplish. After I felt the program was done I put it up on Heroku so it could tweet every 2-5 hours. The twitter handle is @philosorhymes






