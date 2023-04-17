---
layout: post
title: "The Story Our Music Tells"
author: Maddie Portrey
description: The riveting conclusion to my Spotify data scrape and exploration
image: /assets/images/etienne-girardet-EP6_VZhzXM8-unsplash.jpg
---

I'm sure everyone has been on the edge of their seats since my [last post](https://maddiekkay.github.io/my386blog/2023/03/30/spotify-EDA.html), and for good reason. Who DOESN'T want to know anything and everything about my music library? 

So fine, FINE, I'll give the people what they want. Let's get into my Spotify story.

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/ardian-lumi-6Woj_wozqmA-unsplash.jpg" alt="" style="width:500px;"/>
</p>

We started this journey by scraping my saved songs on Spotify (over 700 songs) and gathering the musical qualities about each song. I wondered what my songs had in common -- why I liked these specific songs. Was there a common thread? What were the songs that fell close to the averages for each category, if any? I cleaned the data and started doing an exploratory data analysis to try and figure out any consistencies among the songs. I decided to focus on the averages of each numerical category, deciding that the songs in the middle two quartiles of each category were the ones I wanted to focus on.

After dividing popularity by 100 to be on the same scale as the other categories, I created boxplots to portray the averages of the following seven categories: popularity, danceability, energy, speechiness, acousticness, liveness, and valence. Displayed below, you can easily see which categories are more spread out and which ones are consistently low or high. Acousticness has the largest range, while speechiness and liveness are consistently low.

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/story.png"/>
</p>

I decided to create a table of the songs that fit in the middle two quartiles (the middle 50% of the data) of each of these six categories, as well as popularity. 


<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/finaltable.png"/>
</p>

I am a big fan of these songs, and I feel like they really do sum up the basics of my music library. Overall, I've enjoyed exploring my music library more in depth and I hope you've enjoyed the journey. Let me know a song that you think sums up your music library below, and thanks for tuning in!

If you want to see the entirety of my code, etc., you can find it [here](https://github.com/maddiekkay/Spotify-Project).