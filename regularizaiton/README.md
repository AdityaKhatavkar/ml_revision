# Regualrization

    Regularizaiton is a technique in which you add the extra information in your data so that it dont overfit.

    Regularization adds a penalty term to the loss function used to train the model.


# Where should we use it.

    It is specially  used in regression problems.


#  Three kind of regularization are there generally.

    1. Ridge regularization (L2 Regularization)
    2. Lasso regularization (L1 Regualarization)
    3. Elastic Net


#  Ridge Regression

    sum (0->n) ( (y - y_hat)^2 +  lambda * sum (0->n) (Wi^2))

    1> How the coefficients get affected ?

        If we start increasing the lambda value then all the coefficients get reduces/shrinked, get close to zero. But never becomes zero.

    
    2> Higher values  are impacted more.

        Suppose, we have w1 = 1000, w2=100, w3=1

        If we increase value of lambda.

        Here w1 will decrease more as compare to w2 and w3 will reduces as high reate than w3.

        Higher the values, values get impacted more.

    
    3> Bias Variance Tradeoff
    
        As lambda increases, many times helps to reduce overfitting.
        Hence bias also increases and variance decreases.

# Lasso Regression

    Loss = MSE + lambda* (sum(absolute(w)))

    1> How the coefficients get affected ?

        In L1 Reguralization, as lambda or alpha increases then values of coefficient may get reduct to '0' unlike in L2 reguralizaiton.

        Consider we have high dimensional data and we opted to little greater values of lambda/alpha. In case of polynomial regression some of the coeffecients will get zero. Some features get cutt down and rest features get selected.
        Hence L1 regularization also works as feature selector. 
        That is why L1 regu. is preferred over L2 regularization.


    2> Similiar to Ridge Regression, in Lasso regression higher values are impacted more.


    3> Impact on bias and variance. 

        As lambda increases, many times helps to reduce overfitting.
        Hence bias also increases and variance decreases.

