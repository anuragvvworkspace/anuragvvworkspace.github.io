# Revision Post first 6 lectures

## Lecture 1:
prediction function
  - predicts output y given input x
training data
  - a set of (input x, output y) pairs
supervised learning algorithm
  - takes training data and produces a prediction function 
  
  

Types of classification
* Binary classification
* multi-class classification
* probabilistic classification or soft classification
* regression

How to Convert Categorical Data to Numerical Data?
This involves two steps:

Integer Encoding
One-Hot Encoding( read on this (here)[https://machinelearningmastery.com/why-one-hot-encode-data-in-machine-learning/])

Evaluation of prediction function
Loss function


Splitting data into training and testing
Importance of test set. Should be used only in the last stage before deployment, even if you have multiple ML methods to test.

k-Fold Cross validation
Cros validation for time series

Caveats while learning
Leakage
Nonstationarity
  * covariant shift
  * Concept drift
  
  Model complexity
  Over fitting
  
## Lecture 3(coz lecture 2 is case study)
#### Statistical Learning Theory

Formalization of the Learning Problem  
Three spaces Input space X, Action space A, Outcome space y  
what are the spaces for logistic regression, linear regression, SVM?  

How to evaluate prediction function?  
Risk = Expected loss;  
But we do not know P(x,y) the probability in real life. We work around this by estimating P  
Baye's Decision Function that minimizes risk.  
Finding baye's function for least square regression.  
. Do homework  
    .. Derive bayes function for least square regression | Understand it thoroughly.  
    .. find bayes for other functions  
        
