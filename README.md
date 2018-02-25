Kaggle - Predictive Analytics for Social Impact (WiDS 2018 Datathon)
==============================

#### Intro

This Readme file is for Datawraiths of Aotearoa team entry for the [Predictive Analytics for Social Impact](https://www.kaggle.com/c/wids2018datathon), hosted by Kaggle with the Women in Data Science Conference (WiDS)

The WiDS Datathon is intended to encourage women data scientists to participate in predictive analysis contests. Teams must be majority women to enter.

The challenge is to use demographic and behavioural information from survey respondents in India on their use of traditional and mobile financial services to predict the gender of respondents. 
Ideally, this data can then be used to help enable more Indian women to access financial services. 

#### Packages

Executing this benchmark requires R along with the following packages:


+ library(dplyr)       # 0.7.4    data manipulation
+ library(tidyr)       # 0.8.0    used for data tidying in conjunction with dplyr
+ library(reshape2)    # 1.4.3    used for the melt function
+ library(mice)        # 2.46.0   multivariate imputation
+ library(caret)       # 6.0-78   classification and regression training
+ library(ggplot2)     # 2.2.1    nice plots
+ library(xgboost)     # 0.6.4.1  gradient boosting
+ library(h2o)         # 3.16.0.2 deep learning    
+ library(e1071)       # 1.6-8    support vector machines
+ library(Hmisc)       # 4.1-1    labelling columns of dataset
+ library(data.table)  # 1.10.4-3 faster data extraction functions
+ library(xlsx)        # 0.5.7    reading excel data
+ library(mlr)         # 2.11     machine learning
+ library(Boruta)      # 5.2.0    feature selection
+ library(VIM)         # 4.7.0    visualising imputation
+ library(stringr)     # 1.2.0    string operation wrappers
+ library(vtreat)      # 1.0.2    dataframe
+ library(FactoMineR)  # 1.39     multivariate data mining
+ library(unbalanced)  # 2.0      racing for unablanced methods selection
+ library(fastcluster) # 1.1.24   fast hierarchical clustering

#### How to

To run the benchmark,

1. [Download the data](https://www.kaggle.com/c/wids2018datathon/data)
2. Modify SETTINGS.json to point to the training and validation data on your system, as well as a place to save the trained model and a place to save the submission
3. Train the model by running `python train.py`
4. Make predictions on the validation set by running `python predict.py`
5. [Make a submission](https://www.kaggle.com/c/wids2018datathon/submit) with the output file

This benchmark took approximately 1.5 hours to execute on a Windows 8 laptop with 8GB of RAM and 4 cores at 2.7GHz.
