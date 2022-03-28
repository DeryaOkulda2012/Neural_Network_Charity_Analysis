# Neural_Network_Charity_Analysis

## Overview

Alphabet Soup, is a nonprofit philanthropic foundation dedicated to help various organizations around the world. By building a deep learning neural network with an at least 75% predictive accuracy determining the success or failure of charitable donations to non-profit companies.

This neural network is built to help Alphabet Soup make future decisions on who should receive charitable grants based on historical data. The dataset provided contains information from 34,000 organizations that could potentially be used to build a model with high predictive accuracy.

## Results

### Data Preprocessing

What variable(s) are considered the target(s) for your model?
- IS_SUCCESSFUL: was the money used effectively

What variable(s) are considered to be the features for your model?
- APPLICATION_TYPE: Alphabet Soup application type
- AFFILIATION: Affiliated sector of industry
- CLASSIFICATION: Government organization classification
- USE_CASE: Use case for funding
- ORGANIZATION: Organization type
- STATUS: Active status
- INCOME_AMT: Income classification
- SPECIAL_CONSIDERATIONS: Special consideration for application
- ASK_AMT: Funding amount requested

What variable(s) are neither targets nor features, and should be removed from the input data?

- EIN and NAME: Identification columns

## Original Model

### NN_first_pass_accuracy
!["images/Train_Accuracy.png"](images/Train_Accuracy.png)

### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
* What steps did you take to try and increase model performance?
* Were you able to achieve the target model performance?

Attempt # 1
  * Used original model neurons, layers, and activation functions-changed bin sizes
  * Changed bin sizes for APPLICATION_TYPE and CLASSIFICATION from original model
  * Attempt #1 - Target not achieved
!["images/Attempt1.png"](images/Attempt1.png)

Attempt # 2
  * Increased to 3 hidden layers
  * Added in third hidden layer
  * Attempt #2 - Target not achieved
!["images/Attempt2.png"](images/Attempt2.png)

Attempt # 3
  * Changed activation functions to linear, relu, and tanh
  * Changed activation functions
  * Attempt #3 - Target not achieved
!["images/Attempt3.png"](images/Attempt3.png)

Attempt # 4
  * Increased neurons from 8:5 to 10:8 and changed activation functions from relu:relu to relu:tanh
  * Changed number of neurons and activation functions
  * Attempt #4 - Target not achieved
!["images/Attempt4.png"](images/Attempt4.png)


## Summary

Only one attempt improved the accuracy of the model but did not reach the 75% target. Further exploration and trials would need to be done to find the optimal parameters for a model that achieved an accuracy of 75% or greater
