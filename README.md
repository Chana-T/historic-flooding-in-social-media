# Project 5: Leveraging Social Media to Identify Major Historic Flood Events

## Problem Statement
Floods are one of the most frequent natural disasters, which threaten human and animal life as well as cause significant damage to cities' infrastructure. In order to effectively equip cities to anticipate floods, a deep analysis on vulnerabilties of cities is needed. That said, the impact of major floods on particular cities is difficult to determine due to there being minimal tools accessible to the public that can effectively identify major flood events on a global scale. This study aims to create an open-source tool to identify historical flood events based on data extracted from Twitter and international weather stations.


### Team Members
* [Angeline Lee](https://www.linkedin.com/in/angelinevlee/)
* [Chana Tilevitz](https://www.linkedin.com/in/chanatilevitz/)
* [David Li](https://www.linkedin.com/in/davidgnli/)

## Executive Summary
We knew Twitter would provide categorical information related to flood disasters. As a way to assess relevant and insightful tweets from unhelpful tweets(i.e. noise), we designated a developed city (Houston, TX) and a developing city (Manila, Philippines) as our use cases. Because floods are prevalent in different types of regions, it was important to choose two cities that could reflect this difference in addition to transcend cultural frames of reference. 

After scraping over 30,000+ tweets and taking a close look at how people tweeted during flood disasters, we found that the frequency of tweets was not always directly correlated to the impact of a flood. This led us to pursue weather data as an objective viewpoint to analyze alongside the user generated tweets.

By leveraging the cdo_api_py, we scraped official weather information from NOAA. We created a flexible function(get_weather) that utilizes several parameters in order to find the desired data. Our function is able to highlight key weather information on a given region within a given date range.

We realized that there could be multiple weather stations in close proximity to one another and therefore we decided to group the data by date and averaged the temperature along with the precipitation collected from those weather stations. 


## Conclusion and Next Steps

Sentiment Analysis on Tweets

Integrate with government disaster agencies

Integrate with satellite imagery

Source from more international weather services

Source from other social media platforms (i.e. region-specific)


### Source Documentation
* [National Oceanic and Atmospheric Administration](https://www.noaa.gov/weather)
* [Houston Disaster That Wasn't](https://www.houstonpublicmedia.org/articles/news/2017/06/22/205744/the-storm-that-wasnt/)
* [Houston Flood 2014](http://floodlist.com/america/usa/thunderstorm-flash-floods-houston-texas)
* [Houston Flood 2015](http://floodlist.com/america/usa/texas-floods-6-killed-after-storms-sweep-through-austin-and-houston)
* [Manila Flood 2014](https://center.noah.up.edu.ph/habagat-2014-flood-marikina-city/)
* [Manila Flood 2016](http://floodlist.com/asia/philippines-floods-manila-central-luzon-calabarzon-august-2016)
* [Manila Flood 2017](https://www.rappler.com/move-ph/issues/disasters/181867-flooded-areas-metro-manila-september-12)
