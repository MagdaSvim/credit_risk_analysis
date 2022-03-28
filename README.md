# Credit Risk Analysis

## Purpose

This project uses various techniques to train and evaluate models with imbalanced classes, as well as a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Financial information

The analysis uses data from customers like loan size, number of loans, interest rate, borrowers' income, number of accounts, derogatory marks and total debt. All this information is used to predict whether the loan is healthy (assigned value 0) or high-risk for default (assigned value 1).

## Basic information about the variables

This project works with two parameters:

 - X data - consits of the variables that the model will use to make pedictions; these variables are sometimes called the **features**

 - y data - is the variable that we want to predict; sometimes it is called the **target**

## Stages of machine learning

 - **Model** - something in the real world; a model starts as untrained that is to be shaped to the data

 - **Fit** - this stage is also known as the training stage; it is adjusting the model so that it matches patterns in the data

 - **Predict** - trained model can be used to predict new data

## Methods used

 - [**LogisticRegression**](https://www.ibm.com/topics/logistic-regression) - is used to understand the relationship between the dependent variable and one or more independent variables by estimating probabilities using a logistic regression equation

 - [**Resampling Method**](https://machinelearningmastery.com/random-oversampling-and-undersampling-for-imbalanced-classification/) - involves randomly selecting examples from the minority class, with replacement, and adding them to the training dataset

---

## Results

Machine Learning Model 1 - **Logic Regression**

 - Balanced accuracy score = 95.2%
 - Precision: 
	- 0 = 100%
	- 1 = 85%
 - Recall:
	- 0 = 99%
	- 1 = 91%

Machine Learning Model 2 - **Random Over Sampler**

 - Balanced accuracy score = 99.3%
 - Precision:
	- 0 = 100%
	- 1 = 84%
 - Recall:
	- 0 = 99%
	- 1 = 99%

---

## Summary

Even though the first model predicts the high-risk loans with slightly higher pecision, the second model predicts the high-risk loans with significantly higher recall. The accuracy score is also significantly higher in the second, resampled, model. As we are more concerned about identifying the high-risk loans, the resampled model seems to be better choice for our analysis.

---

## Technologies

For this project we use the following tools:

* [conda](https://github.com/conda/conda) -  cross-platform, language-agnostic binary package manager

* [pandas](https://github.com/pandas-dev/pandas) - is a Python package that provides fast, flexible, and expressive data structures designed to make working with "relational" or "labeled" data both easy and intuitive 

* [Scikit-learn](https://scikit-learn.org/stable/) - is widely used for classification, predictive analytics, and very many other machine learning tasks

---

## Instalation Guide

Before opening the Jupyter notebook, you need to install:

```python
conda install -c conda-forge imbalanced-learn
```

```python
conda install -c conda-forge pydotplus
```

---

## Contributors

Author: Magdalena Svimberska
email: magdalena.svimberska@gmail.com

---

## License

GNU General Public License