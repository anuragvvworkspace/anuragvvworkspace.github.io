### 2:00
Hypothesis space for Linear regression

|F = {f(x) = w^t*x | for all w belongs to R^d }

risk R(f) * = E[l(f(x),y)] = expected value of (loss of (f(x) and y))
          * = E(f(x)-y)^2
          * = E(w^t*x - y)2 
Emperical risk R_hat = 1/n*sum(w^t*x-y)^2

Now we need to do ERM. How?

Find f that minimizing the Emperical Risk. Meaning find optimal w since f is function of w

Objective function is the function to minimize here

## Unconstrained Optimization

### Convergence Theorem for fixed Step Size

||delf(y)-delf(x)|| < L*||y - x||  #Lipschitz constant 

Then gradient descent with fixed step size t <= 1/L converges.

Gradient Descent for Linear Least Square Regression 

risk R(f) = E[l(f(x),y)]

We need to find the optimal f to minimize risk ie minimize over w.

applying del on both sides.
del R_hat(w) =  1/n*sum(del(w^t*x-y)^2)

###minibatch training
We can use minibatch to avoid all the data. 

*Note*: The lecture talks about how the minibatch could be an estimate of the larger data and how bogger the minibatch better the estimate. But i did not listen to the statistics. 

last slide skipped. Check it out for completion.

Conclusion

