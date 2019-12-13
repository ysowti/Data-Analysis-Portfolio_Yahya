# Data Science Portfolio

## Data Analysis Projects

### Stock Market Analysis

In this portfolio project I look at data from the stock market, particularly some technology stocks. I use pandas to get stock information, visualize different aspects of it, and finally look at a few ways of analyzing the risk of a stock, based on its previous performance history. I also predict future stock prices through a Monte Carlo method.

### 2016 Presidential Election Data Analysis

In this data analysis project I am looking at data from 2016 election and analyze two datasets. The first dataset I analyze is the results of aggregated political polls to answer some questions like the party affiliation of people being polled, the effect of undecided polls, change of polls sentiment over time and the effect of debates on polls. The second dataset I use is donors dataset to statistically analyze the donation amount and see how it differs between candidates and parties, trying to find demographics of donors and to find patters in donation amounts.


## Cardiologists Detection Problem

Detect Cardiologists

Assume, you are working for a large marketing firm that targets doctors based on their practice area. Your current campaign is targeting Cardiologists, and you are tasked with coming up with a list of doctors to contact.
You are given a file, physicians.csv, which contains a list of doctors and their unique specialty. You notice that there are a decent number of doctors with "Cardiology" as a specialty, but there are also quite a few doctors whose specialty is "Unknown". You wonder if any of these doctors might actually be Cardiologists.
You find a public dataset, procedures.csv, which contains a list of procedures your doctors performed over the past year. This dataset includes procedures that these doctors performed over the past year, and also number of patients.
The goal is that using this procedure data, determine how many of the doctors with unknown specialty were actually cardiologists.

I answer this question using two techniques:

### Detect Cardiologists using NLP:

In solution 1, I use natural language processing to mine information in procedure column and classify physicians to cardiologists and non-cardiologists based on Naive Bayesian Classifier.

### Detect Cardiologists using Random Forest classification:

In solution 2 I use procedure code column and use Random Forest classifier to classify physicians and do a thorough evaluation of the model based on cross validation, precision/recall trade-off as well as AUC.


## Diagnosis Problem

In this problem, the goal is to build a ML model that predicts diagnosis based on symptoms and other factors. As input csv file we have data_challenge.csv that contains a number of medical cases (extracted from EHRs). Each entry consists of:

- one or more “present” symptoms (symptoms that patient had at the time of visit). For example s_0136 is the code for “earache”.
- one or more “absent” symptoms (symptoms that patient did not have). Note that there may be other potential symptoms the patient was never asked about, which are neither “present” nor “absent”
- Age, Sex (1=Male), and Month of visit (which may be helpful, e.g. some conditions are gender-specific, some are seasonal).
- Diagnosis (“DX”) the patient was diagnosed with (using Gyant condition codes)

I solve this problem using two different techniques:

### Diagnosis prediction using NN:

In this solution I used Keras and deep learning to solve the multi-class classification problem and used sample weight capability of Keras in order to have a model that performs more evenly across different classes in order to deal with unbalance dataset.

### Diagnosis prediction using XGB:

In this solution I did some explanatory data analysis and data visualization and used XGBoost model to predict the diagnoses and dealt with imbalanced dataset.

## NLP Project


