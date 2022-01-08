# Predicting Electric Rotor Temperature 
**Author**: Dahye Kim 
**Last Edited**: 23 Apr 2021 
**Programming Language**: R 
**Libaries Used**: `readr`, `ggplot2`, `reshape2`, `caret`, `glmnet`, `randomForest`, `tidyverse`, `plotmo`, `glmnetUtils`

## Introduction

This program creates series of machine learning models to predict electric motor temperature using various features, including the electric current and voltages, temperature of the ambient and ambient. It first starts off by loading in the data and explore the structure of the data set. Then an extensive exploratory data analysis is performed to inspect the distribution of each attribute in the data set, as well as relationship between each variable pairs. After the EDA, the training data set is fit into numbers of non-parametric and parametric regression models in order to predict the electric rotor temperature. For non-parametric model, necessary hyperparmetres are optimised using cross validation methods. For parametric models, apt parameter estimation assumptions are checked before training the parametric models. The assessment of performance of each model is conducted using cross validations. Finally, the test data set is applied to all the pre-trained models for predicting the target. Some interpretations of the training process and test results are included. 

## Structure of the Notebook

1. EDA
* Statistical Characteristcs of Each Variable 
* Relationship between Each Variable 
2. Methodology & Model Development 
* Non-Parametrics 
  * KNN Regression 
  * Random Forest Regression 
* Parametric
  * Multiple Regression 
  * Polynomial Regression 
  * Stepwise Regression 
  * Shrinkage Methods 
    * Ridge Regression 
    * Lasso Regression 
    * Elastic Net 
4. Results and Discussion 
