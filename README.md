# Data-Analysis-Portfolio_Yahya

## Data Analysis Projects

Data Analysis Project 1: Stock Market Analysis

In this portfolio project I look at data from the stock market, particularly some technology stocks. I use pandas to get stock information, visualize different aspects of it, and finally look at a few ways of analyzing the risk of a stock, based on its previous performance history. I also predict future stock prices through a Monte Carlo method!
I am answering the following questions along the way:

1) What was the change in price of the stock over time? 
2) What was the daily return of the stock on average? 
3) What was the moving average of the various stocks? 
4) What was the correlation between different stocks' closing prices? 
5) How much value do we put at risk by investing in a particular stock?
6) How can we attempt to predict future stock behavior?

Data Analysis Project 2: 2016 Presidential Election Data Analysis

In this Data Project I am looking at data from the 2016 election.
In this project, I analyze two datasets. The first data set is the results of political polls. I analyze this aggregated poll data and answer some questions: 

1) Who was being polled and what was their party affiliation? 
2) Did the poll results favor Clinton or Trump? 
3) How do undecided voters effect the poll? 
4) Can we account for the undecided voters? 
5) How did voter sentiment change over time? 
6) Can we see an effect in the polls from the debates?

The second set of questions I am trying to answer while looking at donor Data set is:

1) How much was donated and what was the average donation?
2) How did the donations differ between candidates?
3) How did the donations differ between Democrats and Republicans?
4) What were the demographics of the donors?
5) Is there a pattern to donation amounts?

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


