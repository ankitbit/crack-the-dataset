# Welcome!



## Introduction

This exercise will mimic a routine day in the life of a data scientist. 
It will cover the tasks such as data loading, dataset cleaning, pre-processing, transformation etc. followed by exploratory data analysis 
for insights which will lead to building of one or more machine learning model(s).

## Loading the dataset

The dataset is available for the purpose of this exercise in the format of a CSV file which can be dowloaded from the link 
`https://www.cs.toronto.edu/~delve/data/boston/bostonDetail.html`. 
This datset contains information about a large number of houses and 
**consider this exercise as a problem of finding similar houses based on an input house.** 

The objective here will be to first develop a concrete understanding of the dataset 
and thereby pre-process and/ or transform the dataset to extract features out of it which maybe serving the purpose of developing a robust machine learning model 
for recommending similar houses based on an input house. 


## Problem definition
Now, just to remain in the context of the problem and understand it before we exploit the data to solve it, 
imagine we provide our machine learning model an input of a house having some features such (X1, X2, X3, ...XN) 
then the machine must be in a position to recommend us the set of houses similar to the aforesaid house. 
This simialrity is based on the ground that all of the recommended houses are also having either some attributes in common or fairly close to each other.

Now, based on the dataset loaded above, consider the following questions and feel free to answer them in your own words. 
Note that, there is no absolute answer for any of them and so, you can use your experience and creativity to as much extent as possible.

**1. What did you infer from the dataset?** 
Elaborate about some of the **most imortant features that are according to you important as per our problem definiton.** 
And if said in other words, elaborate those features which you feel will play an important role in recommendations of similar houses 
based on a given input houses. Also describe the reasons behind such an intuition. 


**2. How do you think we can formulate the problem of recommending similar houses based on a given input startup into a machine learning problem. 
What would be the type of problem i.e. supervised/ unsupervised/ semi-supervised etc? 
Further, elaborate on how do you approach to solve the problem once you have understood the type of the problem.**


## Data Transformation, Pre-Processing and Cleaning

Now, as previously described, each row or instance in the dataset describes an individual house and each column or attribute in that 
row describes a unqiue feature about that particular house. Most of the feature names are self-explanatory (in fact, the whole description of features is already 
there on the page of daatset to allow a better context) and thus describe the information provided by them. 
Now, there maybe some rows that do not contain viable information and act as noise in the context of our problem definition and therefore needs to be dealt with. 
In other words, we would like to highly encourage you to come up with your own creative solutions to clean the dataset (if needed) 
and separate the information from the noise as much as possible without resulting in heavy data loss. 
Also, let us know the individual steps taken by you in this regard along with the reasons.

`File your replies here`


Now, once you have filtered the noisy or redundant rows from the dataset, we would like to see your creativity in pre-precessing the 
feature information before it maybe ready to be served as a lunch for a machine learning model.
**By pre-processing, we basically mean a way to deal with the non relevant features in the context of our problem.** In order to achive that, you may perform some dimension reduction or anytning else that you like.
Remember, you can be as creative as you like and therefore there are no boundaries well defined to pre-process the feature entities. 
Finally, once you're done with it, report us in not more than 200-300 words about how did you achieve this goal and why did you choose the specific method(s).

`File your replies here`


After data cleaning and pre-processing is done, now you may move towards transformation of the data 
in order to achieve the specific goal of building a recommendation tool that can predict a number of similar houses based on a given house. 
Therefore, we would like to invite you to **create a strategy of how you are going to use the cleaned and pre-processed features for building a model later**. 
In this regard, you have absolute freedom to play with the dataset in any manner you like such as-

1. **You may extract any new features that come to your mind and are not available in the present dataset**. 
This feature extraction may use any methods you like such as creating new features from old ones using your own ideas 
to even using some feature extraction methods provided to us using the open source tools. 
However, don't forget to record your operations in writing to let us know what specific features you extracted and what methods did you use to extract.

2. **You may feel free at any stage of your exercise to change the data types of any feature(s) as per your comfort**. 
However, all you need to do is to record your observations and let us know why did you perform that particular operation.

3. Also, at any stage, if you feel like a particular feature is not relevant, 
**feel free to drop any feature from the dataset and record your statement in writing wherever possible about that operation**. 

Finally, don't forget that we don't want to exhaust you while you write your observations and 
thus they can be of any length and certainly not exceeding more than 200-300 words. Feel free to go as in-depth as you like. 
Remember, that it is a learning exercise and you're free to express the best out of your observation skills.

`File your replies here`

Once you are done in with your data transformation and feature extraction and selection exercise, 
you may go ahead with anything else that strikes your mind and had to be done with the dataset. 
But don't forget, all you need to do is to write you actions in about 50-100 words.

`File your replies here`

## Exploratory Analysis

Every data scientist has a moment when it comes to decide between instincts and observations coming out of data. 
**Feel free to explore the data in depth by carrying out exploratory data analysis and report the outcomes in the space below**. 
Again, you can play as you like with the data and be as creative as possible in creating relevant charts, graphics, 
additional variables or even using statistical methods to explore and understand the dataset. 
We are super eager to read how did you decide to make sense of this cool dataset.

`File your replies here`


## Building Models

Once we have the dataset fully prepared about the houses, the final task is about the creation of a machine learning model that 
has the capability of exploiting the value coming out from the dataset which you just transformed into some of the most 
informative features. Now, in order to create a machine learning model we need to train it and for this purpose, 
you are given complete free hand to use any algorithm(s) that comes to your mind or is known to you. 
Also, just as we discussed in the beginning, you are free to deal with the problem in your own way 
i.e. whether you would like to solve it in a supervised or unsuprvised etc. manner. 
**Finally, once you have successfully build your model(s) using the dataset, 
don't forget to report any striking observations that comes to your mind while building the model or while evaluating it in not more than 200-300 words**. 
Remember, you can talk anything from your choice of algorithms to your choice of model validation or cross validation technique and evaluation methods (metrics) etc. as you like. 
We are already super excited to know your ideas!!!!


`File your replies here`
