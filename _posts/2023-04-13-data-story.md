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

After separating the middle two quartiles from the rest of the data, I created boxplots to portray where each of those averages are. Displayed below, you can easily see which categories are more spread out and which ones are consistently low or high. Acousticness has the largest range, while speechiness and liveness are consistently low.

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/story.png"/>
</p>