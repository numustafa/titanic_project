# Titanic Machine Learning Project

In this notebook, I tend to show my skills as a student of Data Science and Machine Learning. This is my first project on [kaggle](https://www.kaggle.com/code/numustafa/notebook4d61069338), and i will apply all of my machine learning knowledge to predict the survivors of the Titanic shipwreck. To improve upon my workflow, i followed the Kaggle Tutorial, Ken Jee's workflow techeniques and ChatGPT for more elaboration.

## Code and Resources Used
Python Version: 3.11
IDE: VSCode
Workflow building: [KenJee](https://github.com/PlayingNumbers)
Typical concept building: [ChatGPT](https://openai.com/blog/chatgpt)

## Understanding Data
* Train and Test data impot
* Investigate NaN's
* Data distribution

## Exploratory Data Analysis (EDA)
* Develop new features
* Data preprocessing 

## Model Building
First, I tried the ML models on baseline and on transformed data. The transformation is done by converting categorical variables into dummy variables. I also split the data into train and tests sets with a test size of 20%.

I tried different models and evaluated them using 5 fold cross validation. I tried three different models:

* Naive bayes - as a baseline for classification task
* Logistic Regression - used for its simplicity and ease of interpretability.
* Decision Trees - Used DT's b/c they are good at handelling categorical data
* K NearestNeighbourhood - I used KNN, because in my opinion, it can classify more accurately based on neighbouring data points
* Random Forest - with the sparsity associated with the data, I thought that this would be a good fit.
* Support Vector Classifier - I used it just to flex my ML skills. 
* Xtreme Gradiant Boost - again I used it to apply my learning
* Soft Voting Classifier - I used it b/c, I think this might give a summarized version of better classification

Later I tuned the model to improve their classification scores


## Model Performance
Here are the Baseline and Tuned performance of all the models

| Model | Baseline | Tuned Performance |
| :- | -: | :-: |
| Naive bayes | 72.2% | N/A
| Logistic Regression | 82.2% | 82.79%
| K NearestNeighbourhood | 80.99% | 82.9%
| Random Forest | 80.8% | **83.4%**
| **Support Vector Classifier** | **83.3%** | **83.35%**
| Xtreme Gradiant Boost | 82.0% | **85.37%**
| Soft Voting Classifier | 82.45% | 84.3%

