---
https://bloomberg.github.io/foml/#lectures
---
# 1. BLACK BOX MACHINE LEARNING

47:13  I wrote the points for lecture previous to this point is in the notes.
Lemme remember roughly.

Types
. Binary classification
. multi-class classification
. probabilistic classification or soft classification
. regression


Data -> ML -> Prediction function

X -> prediction function -> y


X -> feture extraction -> |R^d

labeled/unlabeled data

Loss functions
	0/1 loss
	square loss

testing and training set.

Nonstationarity
	Covarience shift
	Concept drift

50:28 k-fold cross-validation	
	Compute standard error of k folds of data into train and test sets.
	final Test set always used for final deployment of the algorithm. Its used even after choosing an ML among ML algos if u r choosing among many ML algos

1:12:47 Sample bias: Test inputs different(in distribution) from deployment inputs. Basically test was biased

1:15:00 Model complexity and overfitting
hyper parameter(parameter for the ML itself.) 


Overfitting means good train score, poor test score.

In case of over fitting, you can
	. reduce complexity of your model,

	. increase number of train data.

There are ways of controlling complexity of model. (one of them is regularization talked later.)

Hyperparameters control various things
	. model complexity(eg. polynomial order)
	. type of mode complexity (eg. l1 or l2 regularization)
	. optimization algorithm(eg. learning rate)
	. model type (eg. loss fn, kernal type ect)
 

# 2. CASE STUDY: CHURN PREDICTION
---

# 3. INTRODUCTION TO STATISTICAL LEARNING THEORY
Stastical Learning Theory

Typpical sequence of Events
a) Observe input x
b) Take action a
c) observe outcone y

Evaluate action vs outcome l(a,y)

Typically wanna assume outcome independent of action. By not always the case ( like in autonomous cars)



What would the spaces be for linear regression lie in?

Input space x : past data or latest data R^d

Action a : prediction of next value

Outcome : future value




What would the spaces be for logistic regression?

Input space x : past data or latest data R^d

Action a :  or 1 or probability of 1.

Outcome : 0 or 1




What would the spaces be for SVM?

Input space x : past data or latest data R^d

Action a : prediction of next value

Outcome : future value




12:31 Definition of 

                 Decision function or prediction function: gets input X and produces action A
	             
	             Loss function : 
	             
	             Risk: expected loss R on a new example (x,y)
	             
	             Bayes decision fulction: f* = arg f min R(f)    ==== min R(l(f(x),y)) where R is expected loss, f(x) prediction function l() is loss function, y is output.

Lets try derive bayes decision function for a few losses 
19:51 :.

      Least square regression
        loss = (f(x) - y)^2  where a : action , y outcome
        imlies Risk = E[l(f(x))]
        .
        . solve this and turns out that
        .
        (bayes decision function )f* = E[y|x]
        IMPORTANT        20:22 Homework: f* = E(y/x)  find out why. #mathconcept #probablility: expected value in 

      Multi class classification
        loss = 1 if a != y
        Risk = 0*P(a=y) + 1(P(a!=y)
        What will be the right bayes decision function?
        f* = arg max P(y = k|x) meaning a = k,class with the highest probability
        (if u dont undertand how this came about, go to 22:37)
        Note : decision function is a function over an input x
        
        
        
27:10 We did some finding decision functions from expected losses(which is derived frm probability distributions). 
BUTTTT We donno P(y|x) coz who knows real world right? So what to do?
So ML/statistics/data science resorts to taking a sample data of certain distribution.
Strong Law of Large Numbers saves the day. How? i donno google SLLN

at 29:00
Emprical Risk Minimixation
-------------------------
R = AVERAGE OF ALL LOSS =sum(i = 1-n)(l(f(x),y) / n

35:00 is an example of empirical risk minimizer overfitting a sample data from large data. 
(mind you the understanding is a little hazy here as to what ERM is minimizing, is there only one baye's function ect.)
So to avoid such errors like over fitting, we  would like to stick to some smoothness or congruence while designing ERM.

one approach : Constrained ERM
               . minimize emperical risk to a subset called hypothesis space



# 4. STOCHASTIC GRADIENT DESCENT
------------------------------



