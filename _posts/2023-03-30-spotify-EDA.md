---
layout: post
title: "Spott(ify)ing the Musical Similarities"
author: Maddie Portrey
description: Explore the statistics behind my music library with Spotify's API
image: /assets/images/vishnu-r-nair-m1WZS5ye404-unsplash.jpg
---

As [previously mentioned](https://maddiekkay.github.io/my386blog/2023/03/16/Spotify-Data.html), I'm a big music girlie. That has not changed in the few weeks since I originally scraped my music data from Spotify. In fact, I've been to two concerts just this month and I've bought tickets for two more. With that in mind, I continue to wonder why some songs speak to me more than others. Is it a single factor of acousticness? Of danceability? Is it the perfect combination of energy and valence?

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/steve-harvey-QWUCeS2qVoM-unsplash.jpg"/>
</p>

In this post, I'll dive a little deeper into the statistics behind the music saved in my library. Using the Spotify API, I was able to scrape the data about each track in my liked songs, which has over 700 songs. After cleaning the data, each track has the following information (pulled from Spotify's API information):

 - Popularity

 - Acousticness

 - Danceability

 - Energy

 - Instrumentalness

 - Key

 - Liveness

 - Loudness

 - Mode

 - Speechiness

 - Tempo

 - Time Signature

 - Valence

 Full descriptions of each factor are available [here](https://developer.spotify.com/documentation/web-api/reference/get-several-audio-features).

With these measurements in mind, let's get into some cool graphics representing my music:

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/nineplots.png" alt="" style="width:600px;"/>
</p>

The plots above are nine histograms of the features I thought most relevant to my music. A couple of them even look like normal distributions, which is kind of wild, but there are a couple I want to look into more.

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/popularity.png" alt="" style="width:400px;"/>
</p>


<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/clem-onojeghuo-pTeZKi29EYE-unsplash.jpg"/>
</p>

I loved the couple of song recommendations I got on my last post, but this time let me know the last song you listened to! (even if it's from High School Musical)

The last song I listened to: "Lonely" by **The Wldlfe**