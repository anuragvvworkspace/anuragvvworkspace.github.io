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

