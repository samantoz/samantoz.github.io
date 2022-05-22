---
title: "Project 3: Predicting Heart disease using regression analysis"
excerpt: "This project is to do EDA on the data to get an understanding of the different features and how they are related to one another. We are trying to build a classification problem to answer our main question about the chances of having a heart disease."
collection: portfolio
---

## Introduction
World Health Organization has estimated 12 million deaths occur worldwide, every year due to Heart diseases. Half the deaths in the United States and other developed countries are due to cardio vascular diseases. The early prognosis of cardiovascular diseases can aid in making decisions on lifestyle changes in high risk patients and in turn reduce the complications. This analysis intends to pinpoint the most relevant/risk factors of heart disease as well as predict the overall risk using logistic regression and random forest algorithms.

## Research question
We would like to do Exploratory Data Analysis on the data to get an understanding of the different features and how they are related to one another. We would also look at the variables and see if they are related to one another.We are trying to build a classification problem to answer our main question about the chances of having a heart disease.

1) What are the chances of having a heart disease based on the Vital data collected from a patient?
2) What is the most significant predictor for a Heart disease?
3) Is their a correlation between Age and Sex with the chances of having a heart disease?
4) Is there a possibility that based on the analysis of the vital data if we could prevent a possible heart failure from happening?
5) 

## Approach
I am planning to use Logistic Regression algorithm using glm and random forest in order to do a comparison to the output. The random forest algorithm works by aggregating the predictions made by multiple decision trees. I would be using bootstrapped dataset created from the original dataset.

## How my approach addresses (fully or partially) the problem
When the random forest is used for classification and is presented with a new sample, the final prediction is made by taking the majority of the predictions made by each individual decision tree in the forest. In the event, it is used for regression and it is presented with a new sample, the final prediction is made by taking the average of the predictions made by each individual decision tree in the forest.

This is a link to the Readme file and the source code is [**here**](https://github.com/samantoz/dsc680-applied-datascience/blob/main/Project-1/Readme.md)