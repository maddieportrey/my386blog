---
layout: post
title: "Spotify? No, it's SpotiPy"
author: Maddie Portrey
description: Using Spotify to scrape your personal music information
image: /assets/images/mohammad-metri-1oKxSKSOowE-unsplash (1).jpg
---

I'm a big music girlie; I love music. I'm constantly listening to something, and I love finding new music from new artists. But how do I know if I'm going to love a song? Is there some kind of weird algorithm in my brain that's wired to enjoy a song? Luckily, using the Spotify Web API, I can try to find out the answer.

Spotify makes some of its data publicly available through its Web API. This allows anyone who creates a Spotify Developer account and registers an application to access data about users, playlists, tracks, and more. This data is intended to be used by developers to make new applications, tools, and services that enhance the Spotify experience. For someone who is scraping data for non-commercial use, like me, this is considered ethical as long as I'm not infringing on any copyrights or violating any terms of use.

 <p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/clay-banks-fEVaiLwWvlU-unsplash.jpg"/>
</p>

### The Process:

After creating a Spotify Developer account and registering an application to obtain the necessary API credentials, it's time to start coding. With Python, you can use the requests library to make HTTP requests to the API and the json library to parse the response data.

To get started, I used the API's search endpoint to get a user's saved tracks. You can read the full documentation for this endpoint [*here*](https://developer.spotify.com/documentation/web-api/reference/#/operations/check-users-saved-episodes), and explore the other endpoints [*here*](https://developer.spotify.com/documentation/web-api/reference/#/).

 <p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/dominik-vanyi-5Fxuo7x-eyg-unsplash.jpg"/>
</p>

### My work:

 <p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/muneeb-syed-4_M8uIfPEZw-unsplash.jpg"/>
</p>

