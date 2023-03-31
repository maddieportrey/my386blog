---
layout: post
title: "Spott(ify)ing the Musical Similarities"
author: Maddie Portrey
description: Explore the statistics behind my music library with Spotify's API
image: /assets/images/vishnu-r-nair-m1WZS5ye404-unsplash.jpg
---

As previously mentioned, I'm a big music girlie. That has not changed in the few weeks since I originally scraped my music data from Spotify. In fact, I've been to two concerts just this month and I've bought tickets for two more. With that in mind, I continue to wonder why some songs speak to me more than others. Is it a single factor of acousticness? Of danceability? Is it the perfect combination of energy and instrumentalness?

In this post, I'll dive a little deeper into the statistics behind the music saved in my library. Using the Spotify API, I was able to scrape the data about each track in my liked songs, which has over 700 songs. After cleaning the data, each track has the following information (pulled from [Spotify's API information](https://developer.spotify.com/documentation/web-api/reference/get-several-audio-features)):

 - Popularity: the popularity of the track. The value will be between 0 and 100, which 100 being the most popular. The popularity is calculated by algorithm and is based, for the most part, on the total number of plays the track has had and how recent those plays are.

 - Acousticness: A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.

 - Danceability: Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.

 - Energy: Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy.

 - Instrumentalness: Predicts whether a track contains no vocals. The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content.

 - Key: The key the track is in. Integers map to pitches using standard Pitch Class notation.

 - Liveness: Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live.

 - Loudness: The overall loudness of a track in decibels. Loudness is the quality of a sound that is the priary psychological correlate of physical strength (amplitude). Values typically range between -60 and 0 db.

 - Mode: Mode indicates the modality (major or minor) of a track. Major is represented by 1 and minor is 0.

 - Speechiness: Speechiness detects the presence of spoken words in a track.The more exclusively speech-like the recording, the closer to 1.0 the attribute value.

 - Tempo: The overall estimated tempo of a track in beats per minute.

 - Time Signature: An estimated time signature. The time signiture ranges from 3 to 7 indicating the time signatures of "3/4" to "7/4".

 - Valence: A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).

With these measurements in mind, let's get into some cool graphics representing my music: