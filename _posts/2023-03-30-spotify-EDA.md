---
layout: post
title: "Spott(ify)ing the Similarities"
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
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/nineplots.png" alt="" style="width:500px;"/>
</p>

The plots above are nine histograms of the features I thought most relevant to my music. A couple of them even look like normal distributions, which is kind of wild, but there are a couple I want to look into more.

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/popularity.png" alt="" style="width:500px;"/>
</p>

I created a more detailed histogram of the popularity of each song in my library. In the little histograms above, it looks like most of the songs are round the 50-ish popularity line. In the second one, though, we can see that it was only distributed that way because of how many bins there were. In reality, there are many more songs around the 0 mark than stacked on the 50.

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/valence.png" alt="" style="width:500px;"/>
</p>

Because that plot was so different, I was interested in how the valence plot changed as well. Valence, in this dataset, is a measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sounds more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry). My new valence histogram is very similarly distributed to the littler one above, but it looks like the peak is around .3. I didn't know I listen to more negative music, on average, but it's kind of fun to know.

Speaking of averages, I wanted to know the means of each variable:

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/meantable.png" alt="" style="width:200px;"/>
</p>

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/clem-onojeghuo-pTeZKi29EYE-unsplash.jpg" alt="" style="width:500px;"/>
</p>

I loved the couple of song recommendations I got on my last post, but this time let me know the last song you listened to! (even -- or especially -- if it's from High School Musical)

The last song I listened to: "Lonely" by **The Wldlfe**