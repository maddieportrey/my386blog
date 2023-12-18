---
layout: post
title: "NFL Success and College Conference"
author: Maddie Portrey
description: Can we predict which college conference a player is from by their success in the NFL?
image: /assets/images/patrick-ogilvie-GB9XKDZWwp0-unsplash.jpg
---

The NFL has become a passion of mine in recent years, and I love following players throughout their career as they play on different teams with different team dynamics. My love for college football got me thinking, "Do players in more competitive college conferences do better in the NFL?"

In this post, I'll attempt to dive into why (or why not) college conference matters for players in the NFL.

To start, here are the [college football conferences](https://247sports.com/longformarticle/college-football-power-rankings-sec-remains-toughest-conference-ahead-of-2023-season-per-phil-steele-212568334/#2194030) ranked by difficulty as of June, 2023:

#1. Southeastern Conference (SEC) -- The SEC has produced 13 of the past 17 national chamion, including each of the last four.

#2. Big Ten -- The Big Ten has produced at least one College Football Playoff participant in seven of the nine years since the four-team format began in 2014-15.

#3. Pac-12

#4. Atlantic Coast Conference (ACC)

#5. Big 12

#6. American Athletic Conference (AAC)

#7. Independents

#8. Sun Belt Conference

#9. Mountain West Conference

#10. Mid-American Conference (MAC)

Honorable mentions: Big Sky Conference and The Ivy League

With this in mind, I began to compile datasets to measure success in the NFL while connecting players with their college conference.

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/ameer-basheer-Yzef5dRpwWg-unsplash.jpg" alt="" style="width:500px;"/>
</p>

I pulled data from several datasets, needing player stats, colleges, and conferences. I worked through many ways of doing this, but after data cleaning I finally landed with a dataset that included players from 1950 to 2017, with each row corresponding to a year of their career. I filtered out players who has less than 100 yards during that season, and cut out small conferences that only had a few players because of old conferences or being division II schools, etc.

After setting up the data, I created a few plots to show the difference between yardage and TDs for each conference.

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/conferences by yardage.png" alt="" style="width:500px;"/>
</p>

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/conferences by TDs.png" alt="" style="width:500px;"/>
</p>

I spoke to a couple of my peers and they suggested I create multiple plots to show the frequency of number of yards by conference. The plots are below:

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/yards sep by conf.png" alt="" style="width:500px;"/>
</p>

After looking at the data, I decided to explore a few machine learning models.
