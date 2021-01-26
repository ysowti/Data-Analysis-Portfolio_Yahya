# Data Science Portfolio


## 1 - Mulitlabel multiclass classification with Deep Learning

In this problem we are given a set of service names with their corresponding service categories related to beauty services in training data. Each instance with the given service_name is assigned to one or more categories separated by comma in service_category field. As a results, considering that there are one or more than one categories assigned to each service name, this problem is considered multilabel multiclass classification. To solve this problem I used NLP and word embedding on the input data after preprocessing and vectorized the output data, that then used to trained stacked LSTM model for classification.

## Model: 

I used stacked two-layer LSTM with an embedding layer on top and a dense layer for classification as the last layer. Embedding layer allows to convert tokenized input text into embedded vectors and learns these word vectors jointly with the main task. LSTM or in general RNN works well with sequence data like text. The main reason that two layer LSTM or stacked LSTM is used here is to give model more capacity to learn compared to one layer LSTM. Dropout layers are used each after every LSTM layer to fight overfitting. Finally, the dimension dense layer is the output layer with the number of categories as its number of outputs. For dense layer sigmoid is used as activation function assuming that occurrence of each category does not depend on occurrence of others.

## Metric:

The metric I used is micro averaged F1-socre to evaluate performance of trained model on the validation set. To choose the best threshold value and use it to predict categories, the one that results in the best micro-averaged f1-score based on prediction on the validation set is chosen. The best f1-score that I achieved on the validation set was 0.72 with precision of 0.74 and recall of 0.70 having both higher than 70% with the chosen threshold of 0.3.

## Inference:

Using the model that is trained base on all of training data, predictions are generated on testing data. After adding these predicted multilabel categories to the service names given in testing data, a new file called testing_data_with_predictions.csv is created. The trained model that is used to generate predictions is placed in folder multilabel-LSTM-model and stored in Tensorflow pb format.


## 2 - Diagnosis Problem

In this problem, the goal is to build a ML model that predicts diagnosis based on symptoms and other factors. As input csv file we have data_challenge.csv that contains a number of medical cases (extracted from EHRs). Each entry consists of:

- one or more “present” symptoms (symptoms that patient had at the time of visit). For example s_0136 is the code for “earache”.
- one or more “absent” symptoms (symptoms that patient did not have). Note that there may be other potential symptoms the patient was never asked about, which are neither “present” nor “absent”
- Age, Sex (1=Male), and Month of visit (which may be helpful, e.g. some conditions are gender-specific, some are seasonal).
- Diagnosis (“DX”) the patient was diagnosed with (using specific condition codes)

I solve this problem using two different techniques:

### Diagnosis prediction using Neural Networks:

In this solution I used Keras and deep learning to solve the multi-class classification problem and used sample weight capability of Keras in order to have a model that performs more evenly across different classes in order to deal with imbalanced dataset.

### Diagnosis prediction using XGB:

In this solution I did some explanatory data analysis and data visualization that showed how highly imbalaced classes are distributed. I used XGBoost model to predict the diagnoses and deal with the imbalanced dataset. I also used heatmap of normalized confusion matrix to evaluate accuracy of model across different classes that showed by using xgboost model handling imbalanced classes, we could improve accuracy accross different classes regardless of them being abundant or small in size.


## 3 - Spark Deep Learning Pipeline:

In this project I prototyped a spark pipeline integrated with TensorFlow Keras deep learning framework. In order to do this integration I used a python library and an extension to Keras called Elephas. The goal was to build a model in TensorFlow.Keras framework and to create a pipeline on spark that can run this model using Elephas estimator in order to leverage the distributed analytic engine of Spark. The whole process of data ingestion and transformation is automated that includes selection of numeric and categorical features, scaling numerical features, transforming categorical features, with all steps formed into stages of Spark Pipeline. I ran the whole pipeline on typical bank data but it can run on any tabular data, and do all the data ingestion and transformation, feature engineering, model training and deployment and evaluation on validation and test data. I ran this entire project using Google Colab to build a prototype for an upcoming data science projects where the data will be massive. This allows me to do my data ingestion, pipelining, training and deployment on a unified platform and on a much larger Spark cluster.


## 4 - Sentiment Analysis using NLP and Deep Learning

In This project I use Attention mechanism and LSTM to perform sentiment analysis to detect emotions in a text. The idea is to present a text that will be classified as specific type of emotion based on different classes that represent different types of emotions. In this approach using attention mechanism I try to identify main words in each text that can be associated with a specific type of emotion. This notebook is run in Google Colab with hardware accelerator chosen to be GPU. The data I work with in this project is 'emotion.csv' that contains text in each row and an emotion associated with that text.
