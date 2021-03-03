# crack-the-dataset



## Introduction

This exercise will mimic a routine day in the life of a data scientist. It will cover the tasks such as data loading, dataset cleaning, pre-processing, transformation etc. followed by exploratory data analysis for insights which will lead to building of one or more machine learning model(s) which are specific to the problem solving in the domain of a data driven venture capital.

## Loading the dataset

The dataset is available for the purpose of this exercise in the format of a CSV file which can be dowloaded from the link `https://deepdive-ml.s3-eu-west-1.amazonaws.com/datasets/evaluations/startups_around_the+world.csv`. This datset contains information about a large number of startups and **consider this exercise as a problem of finding recommendations of similar startups based on an input startup.** 

The objective here will be to first develop a concrete understanding of the dataset and thereby pre-process and/ or transform the dataset to extract features out of it which maybe serving the purpose of developing a robust machine learning model for recommending similar startups based on the query of a given startup. In order to that, we have written the first few lines of code that may help you in reading the dataset and making a sense out of it.


```python
# read the data file using any appropriate method you desire and print the contents
from pandas import read_csv
df= read_csv('https://deepdive-ml.s3-eu-west-1.amazonaws.com/datasets/evaluations/startups_around_the+world.csv')
df.head()
```

Now, just to remain in the context of the problem and understand it before we exploit the data to solve it, imagine we provide our machine learning model an input as UBER- a ride sharing startup, then the machine must be in a position to recommend me the set of startups similar to UBER such as OLA CABS, LYFT, GRAB, HEETCH etc.

Now, based on the dataset loaded above, consider the following questions and feel free to answer them in your own words. Note that, there is no absolute answer for any of them and so, you can use use experience and creativity to as much extent as possible.

**1. What did you infer from the dataset?** Elaborate about some of the **most imortant features that are according to you important for recommending of similar startups based on an input startup.** And if said in other words, elaborate those features which you feel play an important role in recommendations of similar startups based on a given input startup. Also describe the reasons behind such an intuition. 


**2. How do you think we can formulate the problem of recommending of similar startups based on a given input startup into a machine learning problem. What would be the type of problem i.e. supervised/ unsupervised/ semi-supervised etc? Further, elaborate on how do you approach to solve the problem once you have understood the type of the problem.**


## Data Transformation, Pre-Processing and Cleaning

Now, as previously described, each row or instance in the dataset describes an individual startup and each column or attribute in that row describes a unqiue feature about that particular startup. Now, there maybe some rows that do not contain viable information and act as noise in the context of our problem and therefore needs to be dealt with. In other words, we would like to highly encourage you to come up wiht your own creative solutions to clean the dataset and separate the information from the noise as much as possible without resulting in heavy data loss. Also, let us know the individual steps taken by you in this regard along with the reasons.

`File your replies here`


Now, once you have filtered the noisy or redundant rows from the dataset, we would like to see your creativity in pre-precessing the textual information before it maybe ready to be served as a lunch for a machine learning model.**By pre-processing, we basically mean a way to deal with the non relevant textual entities in the context of our problem.** Remember, you can be as creative as you like and therefore there are no boundaries well defined to pre-process the textual entities. You maybe using conventional methods such as stop-words filtering, lemmetization or stemming or relatively newer methods such as extracting entities using word embeddings and we are totally fine with your approach as long as it's readable and practically implementable. Finally, once you're done doing it, report us in not more than 200-300 words about how did you achieve this goal and why did you choose the specific method(s).

`File your replies here`


After data cleaning and pro-processing is done, now you may move towards transformation of the data in order to achieve the specific goal of building a recommendation tool that can predict a number of similar startups based on a given startup. Therefore, we would like to invite you to **create a strategy of how you are going to use the cleaned and pre-processed features for building a model later**. In this regard, you have absolute freedom to play with the dataset in any manner you like such as-

1. **You may extract any new features that come to your mind and are not available in the present dataset**. This feature extraction may use any methods you like such as creating new features from old ones using your own ideas to even using some feature extraction methods provided to us using the open source tools. However, don't forget to record your operations in writing to let us know what specific features you extracted and what methods did you use to extract.

2. **You may feel free at any stage of your exercise to change the data types of any feature(s) as per your comfort**. However, all you need to do is to record your observations and let us know why did you perform that particular operation.

3. Also, at any stage, if you feel like a particular feature is not relevant, **feel free to drop any feature from the dataset and record your statement in writing wherever possible about that operation**. Although it is not mandatory to mention all such dropped features in writing.

4. And, 

Finally, don't forget that we don't want to exhaust you while you write your observations and thus they can be of any length and certainly not exceeding more than 200-300 words. Feel free to go as in-depth as you like. Remember, that it is a learning exercise and you're free to express the best out of your observation skills.

`File your replies here`

Once you are done in with your data transformation and feature extraction and selection exercise, you may go ahead with anything else that strikes your mind and had to be done with the dataset. But don't forget, all you need to do is to write you actions in about 50-100 words.

`File your replies here`

## Exploratory Analysis

Every data scientist has a moment when it comes to decide between instincts and observations coming out of data. **Feel free to explore the data in depth by carrying out exploratory data analysis and report the outcomes in the space below**. Again, you can play as you like with the data and be as creative as possible in creating relevant charts, graphics, additional variables or even using statistical methods to explore and understand the dataset. We are super eager to read how did you decide to make sense of this cool dataset.

`File your replies here`


## Building Models

Once we have the dataset prepared about the starrups, the final task is about the creation of a machine learning model that has the capability of exploiting the value coming out from the dataset which you just transformed into some of the most informative features. Now, in order to create a machine learning model we need to train it and for this purpose purpose, you are absolutely free to use any algorithm(s) that comes to your mind or is known to you. Also, just as we discussed in the beginning, you are free to deal with the problem using your own way i.e. whether you would like to solve it in a supervised or unsuprvised etc. manner. **Finally, once you have successfully build your model(s) using the dataset, don't forget to report any striking observations that comes to your mind while building the model or while evaluating it in not more than 200-300 words**. Remember, you can talk anything from your choice of algorithms to your choice of model validation or cross validation technique and evaluation methods (metrics) etc. as you like. We are already super excited to know your ideas!!!!


`File your replies here`

## Explaining Models

One of the most important parts of the life of a data scientist nowadays is the ability to explain how and why the models built by him/ her take certain decisions. And in order to achieve this obejctive, there are a number of model explanation methods avaialble to us. **In this final exercise, you are expected to use your imagination and make the best exploitation of any open source available methods to interpret and explain the decisions taken by your model and don't forget, you can also try any new ideas that comes to your mind while interpreting the outcomes of the two binary classes in a random manner**. Finally, report your outcomes in not more than 200-300 words to make us aware about what did you observe about your model behaviour and which methods did you use to explain your model's decisions and why.

`File your replies here`
