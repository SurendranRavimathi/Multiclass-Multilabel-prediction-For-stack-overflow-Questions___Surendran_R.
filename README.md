# Multiclass Multilabel Prediction For StackOverflow Questions

## Author : Surendran R

**Data set** : https://www.dropbox.com/s/5721wcs2guuykzl/stacksample.zip?dl=0

**Objective** : Given text for Questions from StackoverFlow posts, predict tags associated with them.

This is a scaled down version of predecting only top 10 most occurring tags

**Programming Language** : Python 

**Model Architecture** : Deep Learning using CNN (Conv1D )

**About Data Set**

Dataset has text of questions, answers and thier corresponding tags from the Stack Overflow programming Q&A website.

This is organized as three files:

Questions contains the title, body, creation date, closed date (if applicable), score, and owner ID for all non-deleted Stack Overflow questions.

Tags contains the tags on each of these questions.

Answers contains the body, creation date, score, and owner ID for each of the answers to these questions. The ParentId column links back to the Questions table. We don't use this file as we want to predict Tags given a question

#**Steps:**

## Step 1:**Downloading the data set**

1.   unzipping the data set
2.   Loading the data into data frame as follows


*   questions_df
*   answers_df
*   tags_df






## Step 2: **Reducing the problem statement into top 10 tags**

## Step 3: **Data Pre-processesing**

1. Preparing the contents of data frame 

*   Removing the html tags of Body column in questions_df
*   Merging the Title and Body column in question_df
* Filtering the Top 10 taged questions_df and merging the question_df & tags_df
*Droping ununcessary columns


2.   Label Creation

*   Tokenization

3.   Spliting the data into Train & Test 












## Step 4 : **Model building**




*   CNN (Conv1D) is used 






## Step 5: ***Evaluvation ***

## **Loss**: 0.1140  , **Categorical_accuracy**: 0.7552 



