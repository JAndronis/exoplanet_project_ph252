# Introduction to Data Science and Machine Learning - Project Proposal

## Introduction

Exoplanet parameter estimation is an important part of exoplanet classification and analysis, but it is a complex field with multiple models based on parameter types and ranges. Mass and Radius are two fundamental parameters of exoplanets but are rarely known simultaneously for a given subject, and thus deriving a relationship between the two is very beneficial for further analysis.

## Aims

We aim to implement a machine learning pipeline that will derive the radius of a planet given values like its mass, semi-major axis, the host star's effective temperature or its luminosity.

## Methods

We will initially refine our feature space by using random forests to extrapolate the feature importances and based on those, keep only the relevant features. We will then implement several regression algorithms (LASSO, Ridge, Elastic Net, Random Forests, SVM's) and test their relative performance on our dataset to decide which to include in our pipeline. Randomized Search and Grid Search will be used for optimizing each model. The evaluation of each model will be done by testing its cross validation performance on a test set and by analyzing other metrics like MSE or the $R^2$ score.

## Dataset

We will use data from the Open Exoplanet Catalog, located at https://www.kaggle.com/mrisdal/open-exoplanet-catalogue. It contains 3584 confirmed planets along with various parameters like those mentioned above.
