# Loan Risk Models

## Overview of the Analysis

* The purpose of the analysis is to create a mcahine learning model to identify the creditworthness of borrowers by using lending activity from a peer-to-peer lending service.
* Explain what financial information the data was on, and what you needed to predict. The data includes loans that offer the following information, the loan size, intrest rate of the loan, the borrower's income, debt to income, number of account the borrower has, any derogatry marks, the borrower's total amount of debt and the loan status. What the model will be perdicting are the loan statuses of each laon so in the future the model will be able to tell what will be a healthy or risky loan.
* The data provided 75036 good loans and 2500 bad loans to train our model. 
* Two models were created. The first model used the original data to fit. The second model randomly oversampled so there were an equal amount of healthy and risky loans to fit.
* Both models used Logictical Regression to classify what are considered healthy and risky loans.

---

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * **Acuraccy** ≈ 95%
  * **Precision Scores** Healthy Loans ≈ 100% | Risky Loans ≈ 85%
  * **Recall Scores**    Healthy Loans ≈ 99%  | Risky Loans ≈ 91%



* Machine Learning Model 2(Randomly Resampled):
  * **Acuraccy** ≈ 99%
  * **Precision Scores** Healthy Loans ≈ 100% | Risky Loans ≈ 84%
  * **Recall Scores**    Healthy Loans ≈ 99%  | Risky Loans ≈ 99%

---

## Summary

* The comparing the scores and accuracy of both models, Model 2 performed better. The random reasampling is the major factor to take into account. Depending on how the viewer views random resampling, Model 1 could be seen as better for its ablity to use the original data.
* The reason for Model 1 to not being able to predict Risky Loans correctly is the fact that there are over 30x more Healthy loans than Risky. Intrestingly, when there is an equal amount of Healthy and Risky loans, Model 2 dropped in the precision to correctly predict a Risky loan. 

---


## Technologies

Python version 3.9 
* [pandas](https://pandas.pydata.org/)
* [sklearn](https://scikit-learn.org/stable/)
* [imblearn](https://imbalanced-learn.org/stable/)

---

## Installation Guide

```python
pip install pandas
pip install sklearn
pip install imblearn
```

---

## Contributors

Main contributer **Santiago Hernandez**
- [dsmannight@gmail.com](dsmannight@gmail.com)

---

## License

This application is free for non-profit use.
