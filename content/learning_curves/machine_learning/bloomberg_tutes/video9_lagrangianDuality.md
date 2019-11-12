In this lecture, we will explore lagrangian duality and proove the equivalence (mentioned in previous classes) between
the penalized and the constraint form of optimization, the tikenof and the ivenof, two forms of regularization.
Also, it gives us an insight into what happens with SVM optimization.

Also lagrangian duality will give a lead into next topic which is kernalization.


History of optimization:
. . Early on, it was about linear, non-linear
. By early 2000s
. . it became about convex, non-convex problems.
. . Then stocastic gradient descent magic happened (i lost track)


book - Convex Optimization - by Stephen boyd
Extreme abridgement of above book in the link in the video

In higher dimentions, it gets difficult to visualize to see if the function is convex or non-convex.
S0 you gonna need some math to prove convexity of a function.

General optimization problem  


minimize f_0(x)
subject to f_i(x)<=0, i = 1-m
and         h_i(x)=0 i=1-p

equality can be converted to two inequalities.  
```
But why this aversion towards equality constraints? Have to find out  
```
let an optimizastion problem

minimum f_0(x)
subnect to f_i(x) <=0 i=1-m


Lagrangian for this optimization problem is this

L(x,Lamda) = f_o(x) + sum(i=1-m)lamda_i*f_i(x)
here the lamda_i are called legrange multipliers, also called dual variables

The optimization problem can be stated as the **supremum** of the lagrangian
(cons meaning constrainted to)
sup(L(x,lamda))cons:lamda>=0  =  sup(f_0(x) + sum(i=1-m)lamda_i*f_i(x))cons:lambda>=0

Now minimization problem with constraints can be re-written in the form of minization of the above supremum.
This is called primal form.
p^* = inf(sup(L(x,lamda)))  // inf means infimum

**Now**, the dual optimization problem, ie **Legrangian dual problem** is
swapping inf and sup

d^* = sup(inf(L(x)))


Weak max-min inequality






