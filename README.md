# Coronavirus twitter analysis

## Background

Approximately 500 million tweets are sent everyday.
Of those tweets, about 1% are *geotagged*.
That is, the user's device includes location information about where the tweets were sent from.
The `/data-fast/twitter\ 2020` folder contains all geotagged tweets that were sent in 2020.
In total, there are about 1.1 billion tweets in this dataset.


In this project, I followed the [MapReduce](https://en.wikipedia.org/wiki/MapReduce) procedure to analyze these tweets.
MapReduce is a famous procedure for large scale parallel processing that is widely used in industry.
It is a 3 step procedure summarized in the following image:

<img src=mapreduce.png width=100% />

## Plots

After analyzing the tweets, I then created plots using the lang and country results for the following hashtags: #coronavirus and #코로나바이러스 (which is #coronavirus in Korean). I have provided these plots below, along with a brief explanation of my results.

### Plot 1: Country, #coronavirus

<img
  src="country-coronavirus.png"
  style="display: inline-block; margin: 0 auto; max-width: 300px">

### Plot 2: Country, #코로나바이러스

<img
  src="country-코로나바이러스.png"
  style="display: inline-block; margin: 0 auto; max-width: 300px">

### Plot 3: Lang, #coronavirus

<img
  src="lang-coronavirus.png"
  style="display: inline-block; margin: 0 auto; max-width: 300px">

### Plot 4: Lang, #코로나바이러스

<img src="lang-코로나바이러스.png"
style="display: inline-block; margin: 0 auto; max-width: 300px">>

## Process and Results

The purpose of this project was to analyze the geotagged tweets in the aforementioned folder. My goal, through the MapReduce procedure, was to count the occurences of a specific set of hashtags by two categories: languages and countries. Because one of the most prominent events of 2020 was the Covid-19 pandemic, the 17 hashtags that I analyzed were all related to the Coronavirus (covid19, coronavirus, corona, flu, hospital, etc.). My results from this analysis are stored in the 'viz' folder of this repository. The country files are stored in '/viz/country/' and the language files are stored in '/viz/lang/'. One of the bigger picture purposes of this project was to track the spread of information regarding the coronavirus, in the world. By seeing the geotagged location of the tweets, rough conclusions can be drawn about how Covid-19 information spread throughout the world. 

The results of my plots show the following information:
Plot 1: This plot shows that the United States, India, and the UK were the countries with the highest number of #coronavirus tweets.
Plot 2: This plot shows that the highest number of #코로나바이러스 (which is #coronavirus in Korean) tweets were from South Korea, with no other country remotely comparing. This makes sense, as Korean is the official language of South Korea.
Plot 3: This plot shows that the languages that included the most #coronavirus tweets were English, Spanish, and Portuguese.
Plot 4: This plot shows that the language with the most number of #코로나바이러스 tweets was Korean, which makes sense as #코로나바이러스 is the Korean form of #coronavirus.
