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

### Detect Cardiologists using Naive Bayesian classification:

In solution 1, I use natural language processing to mine information in procedure column and classify physicians to cardiologists and non-cardiologists based on Naive Bayesian Classifier.

### Detect Cardiologists using Random Forest classification:

In solution 2 I use procedure code column and use Random Forest classifier to classify physicians and do a thorough evaluation of the model based on cross validation, precision/recall trade-off as well as AUC.


## Diagnosis Problem

## NLP Project


