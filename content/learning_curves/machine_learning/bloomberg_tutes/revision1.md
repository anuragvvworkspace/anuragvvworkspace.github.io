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
Importance of test set. Should be used only in the last stage before deployment, even if you have multiple ML methods to   test.  

k-Fold Cross validation  
Cross validation for time series

Caveats while learning
Leakage
Nonstationarity
  * covariant shift
  * Concept drift
  
  Model complexity
  Over fitting  
## Lecture 2 is case study. So omitted here. Was there any take aways from the lecture????? You will never know now!!!!  
## Lecture 3 Statistical Learning Theory  

Formalization of the Learning Problem  
Three spaces Input space X, Action space A, Outcome space y  
what are the spaces for logistic regression, linear regression, SVM?  

How to evaluate prediction function?  
###### Risk
Risk = Expected loss;  
But we do not know P(x,y) the probability in real life. We work around this by estimating P  
Baye's Decision Function that minimizes risk.  
Finding baye's function for least square regression.  
* Do homework  
    * Derive bayes function for least square regression | Understand it thoroughly.  
    * find bayes for other functions  
    * For multi class, bayes prediction is the class with the highest probability
    
###### Emperical Risk
Since we do not know the probability of real entities, we can estimate and take a sample from the estimated model.
Risk derived from such sample is called emperical risk. 
Since from STRONG LAW OF LARGE NUMBERS, Expeccted value = average of values in sample set, we have that 
* Emperical Risk R_hat = average of loss over all samples.

## Lecture 4 Stocastic Gradient Descent
#### Revision of Statistical learning Theory on an example linear least squares regression
So basically we have to minimize the emperical risk function. Next is the most popular minimization method called gradient descent.  
#### Gradient Descent
Lipchitz continuity. (basically gradient step must be less than slope(proportionally) ).   
So convergence is garenteed if step size is less than 1/L (L is proportional to slope)  
* Batch gradiend descent(full size of dataset M)
* Minibatch gradient descent(m < M)
* stochastic gradient descent(m = 1)

#### Skipped last three slides. Please conver it for sake of completelness  

## Lecture 5 Excess Risk
Excess risk = Emperical risk - Bayes risk
Approximation error  = Hypothesis Risk - Bayes risk
Estimation error = Emperical risk - hypothesis risk
similarly optimization risk.


## Lecture 6 L1 and L2 Regularization
Skipped this lecture. Have to come back to it.
