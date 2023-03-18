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

To get started, I used the API's search endpoint to get a user's saved tracks. You can read the full documentation for this endpoint [here](https://developer.spotify.com/documentation/web-api/reference/#/operations/check-users-saved-episodes), and explore the other endpoints [here](https://developer.spotify.com/documentation/web-api/reference/#/).

First, you need to establsh connections with your authorizations codes:

```
with open('clientspotify.txt', 'r') as file:
    cid = file.read()
with open('secretspotify.txt', 'r') as file:
    secret = file.read()
client_credentials_manager = SpotifyClientCredentials(client_id = cid, client_secret = secret)
```

My files that contain my authentication keys are called 'clientspotify.txt' and 'secretspotify.txt', but you need to create your own.

Next, I used a loop to get all of my saved tracks. The API endpoint only gets 50 songs at a time, so offsetting the data is necessary:

```
my_tracks = sp2.current_user_saved_tracks(limit = limit, offset = offset)

while(len(my_tracks['items']) > 0):
    for i in range(50):
        if len(my_tracks['items']) >= i+1:
            try:
                current_track = my_tracks['items'][i]['track']
                
                uris.append(current_track['uri'])
                names.append(current_track['name'])
                ids.append(current_track['id'])
                release_dates.append(current_track['album']['release_date'])
                popularity.append(current_track['popularity'])
            except:
                print(i)
                
    offset = offset + 50
    my_tracks = sp2.current_user_saved_tracks(limit = limit, offset = offset)
```

From here, I used another endpoint to retrieve the audio features of each track. After that it's basic data cleaning and wrangling to combine everything into a complete dataframe. [Here's](https://github.com/maddiekkay/Spotify-Project) my GitHub repository with my code and dataset.

 <p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/dominik-vanyi-5Fxuo7x-eyg-unsplash.jpg"/>
</p>

Using the Spotify Web API can be a powerful tool for web scraping and data analysis. With the ability to access data about users, playlists, tracks, and more, I was able to create a complete dataframe of all 700 songs I've saved over the past couple years. Even after just glancing around the dataframe I was immediately able to see some consistencies in different audio features. Stay tuned for the analysis of my saved music and probably some (hopefully) great music recs. Let me know any songs that are taking over your life right now in the comments and they might just make it into my saved songs data frame...

 <p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/muneeb-syed-4_M8uIfPEZw-unsplash.jpg"/>
</p>

My song rec: "The Adults Are Talking" by **The Strokes**