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
,,,
But why this aversion towards equality constraints? Have to find out
,,,


Lagrangian for this optimization problem is this

L(x,Lamda) = 
