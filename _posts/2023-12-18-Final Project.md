---
layout: post
title: "College Conferences and NFL Success"
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

I pulled data from several datasets, needing player stats, colleges, and conferences. I worked through many ways of doing this, but after data cleaning I finally landed with a dataset that included players from 1950 to 2017, with each row corresponding to a year of their career. For each season I had their total number of yards, touchdowns, and number of touches. This was the best way I could find to measure their "success." Success is an arbitrary term, so I decided that I cared about yardage, touchdowns, and touches on the ball. Touches on the ball gives a feel for how much a player actually played in the season. I filtered out players who has less than 100 yards during that season, and cut out small conferences that only had a few players because of old conferences or being division II schools, etc. This did cut out defensive players and likely offensive lineman, but there isn't a fair metric to measure their success against those who are running, catching, and throwing the ball.

After setting up the data, I created a few plots to show the difference between yardage, touchdowns, and touches on the ball for each conference.

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/conferences by yardage.png" alt="" style="width:500px;"/>
</p>

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/conferences by TDs.png" alt="" style="width:500px;"/>
</p>

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/conferences by touches.png" alt="" style="width:500px;"/>
</p>

There doesn't seem to be a huge difference between conferences, with some having higher averages than I would've predicted, like Conference USA in yardage. Part of this could be due to the number of players that come from each conference -- if the SEC has more players get drafted, there are more opportunities for their players to have less playing time, have less yards, and bring down their average.

I spoke to a couple of my peers about what I had explored in the data, and they suggested I create multiple plots to show the frequency of number of yards by conference. The plots are below:

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/yards sep by conf.png" alt="" style="width:500px;"/>
</p>

After looking at the data, I decided to explore a few machine learning models. I looked at Logistic Regression, Random Forest, Support Vector Machines, AdaBoost, and Decision Tree models. I tuned several of the models to give me better results, and all of the accuracy, recall, and precision scores can be seen below:

<p align="center">
<img src="https://raw.githubusercontent.com/maddiekkay/my386blog/main/assets/images/yards sep by conf.png" alt="" style="width:500px;"/>
</p>

The model that had the best scores was ____. It still didn't score super well, which makes me it seem like there isn't a huge correlation between college conference and player sucess in the NFL.

Overall, this was an interesting project to undertake and it helped improve my data cleaning, EDA, and machine learning skills. 