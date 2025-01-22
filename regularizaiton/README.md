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

    We use ridge regression when all features are important and we dont want to remove any of the feature.

    L = sum (0->n) ( (y - y_hat)^2 +  lambda * sum (0->n) (Wi^2))

    i.e  L = MSE + lambda * sum(0->n)(Wi^2)

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

    We use the lasso regression when some of the features are not important so that those featues can be dropped by the lasso regression.

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


    * Lasso Regression in sklearn : 
        
        class sklearn.linear_model.Lasso(
            alpha=1.0, *, fit_intercept=True, precompute=False, copy_X=True, max_iter=1000, tol=0.0001, warm_start=False, positive=False, random_state=None, selection='cyclic'
            )



 # Why lasso regression creates sparisity ? (interview question)

      -> As the lambda incresases, some of the coefficients get reduced to 0. Hence lasso regression creates sparsity in the dataframe.



 # And how does the lasso makes coefficients to zero which is useful for feature selection. And why ridge cant?

     -> Consider x (input) and y(output).
        If we use simple linear regression (without regularizaiton)
          
           y = m*x + b

           m = sum(i-n)[yi - y.mean()][xi - x.mean()] / sum(xi - x.mean())^2

           b = y.mean - m*x.mean

        If we use ridge regression
           b is same. 
           But in formula of m, Lambda is added in denominator.

        If we use lasso regression
            b is same.
            But in formula of m, Lambda is added in numerator.

        Lasso (L1): The penalty  i.e L1 norm forms a diamond-shaped constraint region. The sharp corners of the diamond often align with the coordinate axes, allowing coefficients to hit exactly zero.

        Ridge (L2): The penalty i.e L2 norm forms a circular constraint region. The smooth edges of the circle make it unlikely  for coefficients to hit exactly zero

 

 # Elastic net regression.

    Combinaiton of ridge and lasso regression. 

    Usage 1: Use when large dataset is available. And we cant sure whether the features are important or not.

    Usage 2: We use this when, there is multicolinearity between the input features.



    Loss function : 

        L = MSE +  a * sum(absolute(w)) + b * sum(w^2)

        lambda = a + b

        L1_ration = a / (a + b)

        In sklearn, default values are a = 0.5 and b = 0,5