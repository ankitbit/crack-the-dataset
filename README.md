# crack-the-dataset



## Introduction

This exercise will mimic a routine day in the life of a data scientist. It will cover the tasks such as data loading, dataset transformation, cleaning, pre-processing followed by exploratory data analysis which will lead to building of some machine learning model(s) which are specific to the problem solving in the domain of a data driven venture capital.

## Loading the dataset

The dataset is available for the purpose of this exercise in the format of a CSV file which can be dowloaded from the link `https://deepdive-ml.s3-eu-west-1.amazonaws.com/datasets/evaluations/startups_around_the+world.csv`. This datset contains  information about a large number of startups and **consider this exercise as a problem of finding recommendations of similar startups based on an input startup.** 
`Just to understand the context of the problem, imagine we provide our machine learning model an input as UBER- a ride sharing startup, then the machine must be in a position to recommend me the set of startups similar to UBER such as OLA CABS, LYFT, GRAB, HEETCH etc.`

The objective here will be to first develop a concrete understanding of the dataset and thereby pre-process the dataset to extract features out of it which maybe serving the purpose of developing a robust statistical model for recommending similar startups based on the query of a given startup. In order to that, we have written the first few lines of code that may help you in reading the dataset and making a sense out of it.


```python
# read the data file using any appropriate method you desire and print the contents
# write your code here
from pandas import read_csv
df= read_csv('https://deepdive-ml.s3-eu-west-1.amazonaws.com/datasets/evaluations/startups_around_the+world.csv')
df.head()
```

Now, based on the dataset loaded above, consider the following questions and feel free to answer them in your own words. Note that, there is no absolute answer for any of them and so, you can use use experience and creativity to as much extent as possible.

**1. What did you infer from the dataset?** Elaborate about some of the **most imortant features that are according to you important for recommending of similar startups based on an input startup.** And if said in other words, elaborate those features which you feel play an important role in recommendations of similar startups based on a given input startup. Also describe the reasons behind such an intuition. 


If you observe carefully, the dataset has many rows where each row describes a particular fundraising which the co-founder has raised for his company. There maybe more than one row for each co-founder if he has raised multiple rounds of funds. Now, **the definition of success as per our investment thesis is either the entrepreneur is successful in raising funds more than or equal to 500000 EUR described by the feature `amount` or has atleast raised a Series A round described by the feature `funding_type`**. 


**2. How do you think we can formulate the problem of scoring the ability of an entrepreneur to be successful into a supervised learning problem. What would be the data matrix and label for such a case and how would we create a label out of the existing dataset.**

Hint: How would you like to score the ability of being successful- as a regression problem or as a classification problem. While thinking of a suitable label, you may also think of a creating a label by considering or using two or more features. In case of using more than one features for creating a label for the problem, which features do you think we can consider to use as a label for scoring the ability of the co-founders and why?

## Data Transformation, Pre-Processing and Cleaning

Now, as previously described, each co-founder in the dataset has multiple occurences. Thus, each row describes a particular fundraising which the co-founder has raised for his company. However, we can not work with multiple rows describing an individual entrepreneur since we are going to train our supervised learning algorithm in such a manner that it learns to understand how and why certain individuals are more successful than others where each row in the data will correspond to a unique entrepreneur. 

**Therefore, you have to find a way to group the multiple rows corresponding to an individual entrepreneur in such a manner that the outcome dataset has only one row per individual. Hint: You can think of `split-apply-combine`feature fo pandas which may make your life smoother while doing this task.** 

But again, we are fully comfortable with any method or technique used by you and once you're done doing it, report us in not more than 200-300 words about how did you achieve this goal and why did you choose the specific method.

`File your replies here`


After data transformation is done, now your job is to **create an appropriate label for training our model** and also to **perform the exploratory data analysis using the label and one or more features**. In this regard, you have to augment the dataset and create a label using the following criteria-

Following our investment thesis, as described previously, we have decided to create a label which would be binary in nature taking the two classes- `succeessful`or `struggling`. The criteria to mark an entrepreneur successful is that either he should have raised 5000000 EUR or more in funding amount or atleast a Series A funding round as explained before. Create the label using the aforesaid criterion and name it label.

Now, once you're done creating the label for the dataset, we would highly encourage you to play with the dataset again in such a manner that-

1. **You may extract any new features that come to your mind and are not available in the present dataset**. This feature extraction may use any methods you like such as creating new featires from old ones to even using some feature extraction methods provided to us using the open source tools. However, don't forget to record your operations in writing to let us know what specific features you extracted and what methods did you use to extract.

2. **You may feel free at any stage of your exercise to change the data types of any feature(s) as per your comfort**. However, all you need to do is to record your observations and let us know why did you perform that particular operation.

3. Also, at any stage, if you feel like a particular feature is not relevant, **feel free to drop any feature from the dataset and record your statement in writing wherever possible about that operation**. Although it is not mandatory to mention all such dropped features in writing.

Finally, don't forget that we don't want to exhaust you while you write your observations and thus they can be of any length and certainly not exceeding more than 200-300 words. Feel free to go as in-depth as you like. Remember, that it is a learning exercise and you're free to express the best out of your observation skills.

`File your replies here`

Once you are done in your transformation of the dataframe using your own preferred methods, you may go ahead with cleaning the dataset and pre-processing it by looking for any missing values or anything that strikes your mind and becomes the need of the hour and such and write you actions in about 50-100 words.

`File your replies here`

## Exploratory Analysis

Every data scientist has a moment when it comes to decide between instincts and observations coming out of data. **Feel free to explore the data in depth by carrying out exploratory data analysis and report the outcomes in the space below**. You can play as you like with the data and be as creative as possible in creating relevant charts, graphics, additional variables or even using statistical methods such as correlation to explore the dataset.

`File your replies here`


## Building Models

Once we have the dataset prepared about the entrepreneurs, the final task is about the creation of a statistical model that has the capability of exploiting the value coming out from the dataset. Now, in order to create a statistical model we need the label for training the model which we had created previously along with the non label data matrix which is also available to us.**Finally, you are free now to build your model(s) using the dataset and report any striking observations that comes to your mind while building the model or while evaluating it in not more than 200-300 words**. Remember, you can talk anything from your choice of algorithms to your choice of model valiation or cross validation technique and evaluation methods (metrics) etc. as you like. 


`File your replies here`

## Explaining Models

One of the most important parts of the life of a data scientist nowadays is the ability to explain how and why the models built by him/ her take certain decisions. And in order to achieve this obejctive, there are a number of model explanation methods avaialble to us. **In this final exercise, you are expected to use your imagination and make the best exploitation of any open source available methods to interpret and explain the decisions taken by your model and don't forget, you can also try any new ideas that comes to your mind while interpreting the outcomes of the two binary classes in a random manner**. Finally, report your outcomes in not more than 200-300 words to make us aware about what did you observe about your model behaviour and which methods did you use to explain your model's decisions and why.

`File your replies here`
