# Data Science Portfolio

## Detect Cardiologists

Assume, you are working for a large marketing firm that targets doctors based on their practice area. Your current campaign is targeting cardiologists, and you are tasked with coming up with a list of doctors to contact.
You are given a file, physicians.csv, which contains a list of doctors and their unique specialty. You notice that there are a decent number of doctors with "Cardiology" as a specialty, but there are also quite a few doctors whose specialty is "Unknown". You wonder if any of these doctors might actually be Cardiologists.
You find a public dataset, procedures.csv, which contains a list of procedures your doctors performed over the past year. This dataset includes procedures that these doctors performed over the past year, and also number of patients.
The goal is that using this procedure data, determine how many of the doctors with unknown specialty were actually cardiologists.

I answer this question using two techniques:

### Detect Cardiologists using NLP:

In solution 1, I use natural language processing to mine information in procedure column and classify physicians to cardiologists and non-cardiologists based on Naive Bayesian Classifier.

### Detect Cardiologists using Random Forest classification:

In solution 2 I use procedure code column and use Random Forest classifier to classify physicians and do a thorough evaluation of the model based on cross validation, precision/recall trade-off as well as AUC.