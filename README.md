# Credit Card Default Prediction

This project aims to predict whether a credit card holder will default in the next month.

# File Explanation on Github

This repository consists of several files, namely :

- h8dsft_P1M1_Ahmad Luay Adnani.csv = dataset for this project
- Credit_Card_Default_Prediction.ipynb = This file is the main notebook used to explore dataset and built model
- inference_Card_Default_Prediction.ipynb = Notebook used for testing inference. Inferencing is done on a separate notebook to prove that the model can run on a notebook that is clean of variables

# Brief Summary of Project

The flow of this project, first EDA (Exploratory Data Analysis) to find out the basic picture of the dataset. Second, cleaning and preprocessing of the dataset. Third, Built Classification Models using 7 algorithms (Logistic Regression, SVM, Decision Tree, Random Forest, KNN, Naive Bayes, AdaBoost Classifier ). These algorithms are tested based on their baseline/default parameters, and then `cross-validation` will be applied to evaluate each model based on mean and also standard deviation. `SVM` algorithm using baseline parameters is choosen as Best Model.

# Project Conclusion

- Based on the 85% `accuracy` score on the test set, it can be said that selected model is a **good fit** and also **accurate enough** to classify whether a credit card user will default on their credit card in the next month.

- Although this model has a pretty good accuracy, this algorithm model has slightly low `f1_score`. The slightly low `f1_score` on test set 53.4% is due to imbalanced data in the actual target in the dataset (actual positives are greater than negatives) which causes a low `recall` score.

-  `recall` score of 43% for test set means that this model **only catches 43% of all the defaulters**. Which means **misses 57% of all defaulters**. This is not a good thing for banks that issue credit cards for letting a lot of non-loan-returning credit card defaulters go undetected.


