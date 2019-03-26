---
title: 'Emotable: A Sentiment Analysis Model'
projects: true
layout: post
date: '2019-03-26 19:24:46'
image: "/assets/images/emotable.png"
headerImage: true
author: quai
---

Emotable is a sentiment analysis model trained on tweets from the twitter API. It classifies tweets as positive or negative based on the tweet content. 

I created the training and validation datasets by retrieving tweets from the Twitter API that had certain "positive" or "negative" emoji using a TweetCollector class that I built. I got the list of positive and negative emoji from an [existing dataset](https://data.world/kgarrett/emojis) . I made the assumption that a positive tweet is one that contains a positive emoji and no negative emoji and vice-versa for negative tweets.

To build the model I trained a Long Short Term Memory network on 80% of the data I collected and validated it on the remaining 20%. This was my first machine learning project so I did this by adapting a tutorial for creating a sentiment analysis model for movie reviews from IMDB data. The model achieved 85-90% accuracy on classifying tweets as positive or negative. 

---
Languages/Technologies

- **Numpy, Pandas**: Python libraries for data analysis/manipulation
- **TensorFlow, Keras**: Python libraries for training/building ML models
- **Twitter API**: datasource

---
[see the code](https://github.com/Qlwentt/emotable)