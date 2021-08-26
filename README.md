## Sexual Harassment Classification -SafeCity 
![metoo_0](https://user-images.githubusercontent.com/61196335/131012016-2512378f-289f-4705-b7a5-89ab781b8fc4.jpg)

## Overview
1. As the gender inclusion in society is increasing people becoming more confident to talk about their harassment, one such example is MeToo,
a personal stories and experiences about sexual harassment shared online, one such online forum is SafeCity where you can share incidence anonymously. 
This case study tries to categorize various forms of sexual harassment, based on stories shared on the SafeCity for the labels of groping/touching, ogling/staring, 
and commenting.

2. With the amount of data that is being collected by SafeCity, power of NLP can be used to automate the task which eventually helps victims and authorities 
to speed up the process of filling and reporting sexual violence.

3. Automatic classification, and analysis also helps activist to raise the voice against such violence and relevant policy makers to make such laws 
so that offender does not escape from system and pay the price for the crime committed if proven guilty.

## Business Problem Statement
Predict the type of sexual harassment based on given description for which the incident belongs to one, more or none categories, namely are commenting, 
groping/touching and ogling/staring. For ex. ‘Catcalls and passing comments were two of the ghastly things the Delhi police at the International Airport put me and my friend through. It is appalling that the protectors and law enforcers at the airport can make someone so uncomfortable’ is positive for two labels commenting and ogling/staring.

## Data Set 
Data Source : https://github.com/swkarlekar/safecity 

Research paper : https://arxiv.org/pdf/1809.04739.pdft

The multilabel classification folder consists of train, dev, and test set which have 7201 training samples, 990 development samples, and 1701 test samples 
respectively. This data contains four columns first being description of incident, and other three being sexual harassment is present or not.

1. Description (string): talks about personal story of victim.
2. Commenting (integer): label for description whether it belongs to commenting or not.
3. Ogling/Staring (integer): label for description whether it belongs to ogling/staring category or not.
4. Touching/Grouping (integer): label for description whether it belongs to the touching/grouping category or not.

## Business Constraints
1. No strict latency requirement.
2. Misclassification is problem.

## ML Formulation of Business Problem
The problem of predicting the label given a text description of incident can be solved using NLP techniques both
1. Single – Label Classification: it involves building binary classification model for predicting particular query belong to particular category or not.
2. Multi-label Classification: it involves building multi-label classification model for predicting particular query belong to single or multiple 
label/ category or not, simultaneously.

## Performance Metrices: 

1.Hamming Loss: it is average of all labels of incorrect prediction of each class label ex actual = [1,0,0,1], predict = [1,0,1,1], 
N = data points = 1, L = length of label of identity function, here only 1 at 3rd place changes so L = 1, therefore HL = 1.

Ideally we accept hamming loss = 0, which would imply no error, smaller the hamming loss better is performance.

2. Exact Match Ratio (EMR): it is metric that calculates average of all the labels correctly classified, i.e. not partial correct/incorrect taken into account.

3. 1/0 Loss: 1-EMR

4. Accuracy: proportion of predicted correct labels to total number of labels.

Recall: of all the label belongs to positive class; how many model detect to be positive.

Precision: all the points model predicted positive, how many of than are actually positive.

Macro: gives equal importance to each class or label but that doesn’t’ mean data distribution for each class or label have equal importance.

Micro: calculate metric globally by calculating tp, fn, fp.

5.micro-Precision, micro-Recall, F1-micro (harmonic mean of micro-pre., and micro recall)
primary metric used is f1-micro.

## Best Ml Model
![best ml](https://user-images.githubusercontent.com/61196335/131012569-080d682f-47e0-4bc0-a936-b82f3de1aa5a.JPG)

## Best Dl model
![dl best](https://user-images.githubusercontent.com/61196335/131012615-4a640147-840d-4e2f-857f-15cbbe07d562.JPG)

## Deployment
Building webapp and deploying on local system.

![deploy1](https://user-images.githubusercontent.com/61196335/131005763-dda52cb2-d759-4edd-8d26-477240f405fc.gif)

link to web app : https://share.streamlit.io/nik-cy-dv/strmlit-deploy/main

link to blog : https://medium.com/@nks-cy-dv/sexual-harassment-classification-safecity-419eb1b53531

## connect with me on
<a href='https://www.linkedin.com/in/nikhil-sharma-421b60a6/'> ![alt text](https://img.shields.io/badge/Linkedin-connect-blue)</a>       <a href='mailto:nikhil.niksharma15@gmail.com'> ![alt text](https://img.shields.io/badge/gmail-nikhil.niksharma15%40gmail.com-red)</a>

If you have any query or feedback you can connect with me.

