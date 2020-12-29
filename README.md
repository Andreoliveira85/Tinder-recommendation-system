# Tinder-recommendation-system

## Company's Description 📇

<a href="https://tinder.com/?lang=en" target="_blank">Tinder</a> is of one the most famous online dating application in the world right now. The whole idea is to being able to anonymously swipe right or left on a person to show if you liked her or not. If both person swiped right: *It's a match*! And then you can start chatting! 

This whole concept revolutionized the way young people date. Founder <a href="https://www.crunchbase.com/person/sean-rad" target="_blank">Sean Rade</a> believed that *"no matter who you are, you feel more comfortable approaching somebody if you know they want you to approach them."*

With over 50 million users (80% + from 16 to 34), Tinder's valuation is around $1.4 billion which makes this start-up one of the most famous unicorn in california as of today. 😮

## Goals 🎯
Our goal is to

* Recommend 10 best profiles for a given user 

## Scope of this project 🖼️

The dataset is availabale here:


👉👉 <a href="https://full-stack-bigdata-datasets.s3.eu-west-3.amazonaws.com/Unsupervised_Learning/Tinder_data.zip" target="_blank">Tinder Data</a> 👈👈

The files contain 17,359,346 anonymous ratings of 168,791 profiles made by 135,359 LibimSeTi users. You will find a zip file contained data on gender for each person as well as a rating. 

### Introduction to Recommendation engines 

It is now time to discuss Recommendation Engines. 
There are two types of recommendation engines: 

1. Collaborative Filtering 
2. Content Based 

![](https://miro.medium.com/max/690/1*G4h4fOX6bCJhdmbsXDL0PA.png)


### Collaborative filtering principles 

We start this project with Collaborative Filtering. The idea is to recommend a product based on other users' review. Let u see the idea behind  [this explanatory gif](https://www.kdnuggets.com/2019/09/machine-learning-recommender-systems.html#:~:text=Recommender%20systems%20are%20an%20important,to%20follow%20from%20example%20code.) from KDNugget: 

![](https://miro.medium.com/max/623/1*hQAQ8s0-mHefYH83uDanGA.gif)


Instead of having "products" to recommend, this time, we will recommend people!

### Build a utility matrix 

Our goal is to be able to create a recommandation engine built on a utility matrix like this one <a href="https://towardsdatascience.com/math-for-data-science-collaborative-filtering-on-utility-matrices-e62fa9badaab" target="_blank">utility matrix</a>. This should look something like this: 

<img src="https://full-stack-assets.s3.eu-west-3.amazonaws.com/images/utility_matrix.png"/>

### Machine Learning

TruncatedSVD is the perfect algorithm here gue to the sparsity of the utility matrix! 👏 We will apply this algorithm to reduce dimension and then create a <a href="https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.corr.html" target="_blank">correlation matrix</a> to see which profile are correlated and thefore would be a match!  


## Deliverable 📬

Goals: 

* Have built a utility matrix 
* Have created a correlation matrix 
* Recommend a list of 10 profiles for a random user 



## Code/resources used:
**Python version:** 3.7
**Libraries/packages used:** pandas, numpy, scikitlearn
