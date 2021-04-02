# CZ4032-Data-Mining-and-Analytics
## Programming language: Python
## IDE: Jupyter Notebook
## Overview
+ This project performs data mining and analysis on the credit card transactions dataset obtained from Kaggle. Some popular data mining techniques were explored and adopted to find patterns in the data and thus to detect fraudulence from transactions. 
+ The task is broken down into three steps - data preprocessing, building classification models and results evaluation. 
+ In data preprocessing, we explored the dataset and mainly performed **outlier removal**, **feature selection** and **data oversampling**, which provides the final training and testing sets to various classification models. 
+ In the second stage, we built classification models using four supervised machine learning algorithms respectively - **Logistic Regression**, **Support Vector Machine (SVM)**, **Random Forest** and **Artificial Neural Network (ANN)**, and we tested each model’s performance on the testing set. 
+ Lastly, we evaluated the results from different classification models based on certain metrics and chose the best model for this task.

## Evaluation Metrics
+ Considering the high imbalance of the dataset, accuracy of the model is evaluated based on the following metrics:\
#### Confusion Matrix
+ Three scores are considered: **Precision score**, **Recall** score and **F1 score**.
+ They are computed as follows:\
 `Precision = TP TP+FP`\
 `Recall = TP TP+FN`\
 `F1 Score = 2 * precision * recall precision + recall`
#### Precision-Recall Curve
+ Precision-Recall Curve is suitable for an imbalanced dataset, as it focuses more on the minority class, which in our case is the fraud transactions. And the **Area-Under-Curve (AUC)** score will be considered.

+ In addition, there is a trade-off between precision score and recall score. In this project, in order to detect as many fraud transactions as possible, we will focus more on recall than precision.


### Dataset
#### Download the credit card transaction dataset from Kaggle website as `creditcard.csv`
+ https://www.kaggle.com/mlg-ulb/creditcardfraud


### There are five IPython notebooks implemented for this project.
Each notebook can be run independently.
To reproduce the results for a specific section, run the corresponding notebook.

+ data_preprocessing.ipynb : containing code for data preprocessing.
+ logistic_regression.ipynb : containing code for implementing logistic regression models.
+ svm.ipynb : containing code for implementing support vector machine models.
+ random_forest.ipynb : containing code for implementing random forest models.
+ ann.ipynb : containing code for implementing artificial neuron models.



#### Create a folder named `dataset` under `code` folder, which will contain the following files:
+ creditcard.csv : The original dataset from Kaggle.
+ training.csv : The training set generated after data preprocessing. 
+ testing.csv : The testing set generated after data preprocessing.
