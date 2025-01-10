# Mathematical Transformations:

    Some ML algorithms work better on the normally distributed data (like linear, logistic regression).

    Mathematical transformations, like log(x), sqrt(x), etc. These are to be appilied to the numerical features to make the things easier.

    It is better if the distribution of the data is normal. Probability density function (PDF) should be normal. If it is not normal, then we apply the transformation to make it normal.

    Some examples of mathematical transformations are:
        - log(x)
        - sqrt(x)
        - reciprocal
        - power
        - boxcox
        - yeo johson

How we come to know the distribution is normal or not:
        - ditplot in seaborn
        - pandas skew method
        - qq plot (most reliable method)


# Functions transformers : 

            In sklearn
            - FunctionTransformer ----> log, reciprocol, sqrt, custom, etc.
            - PowerTransformer  ------> boxcox, yeo johson
            - QuantileTransformer
        

Log transform: 
    
    We take log of each value in the feature. Thats it.
    When to use: - When the data is not contain negative values.
                 - When data is right skew 



Reciprocal transform (1/x):

    We take reciprocal of each value in the feature. 
    Think it, bigger values becomes small and vice versa.



Square transform: (x^2):

    We take square of each value in the feature.
    When to use : When data is left skew



Square root transform: (sqrt(x)):

    We take square root of each value in the feature. Thats it.



# Power Transformations

Box Cox: 
    
    Two datascientists named Box and Cox collabarated together and developed this technique. 
    Hence called boxcox transformation.
    It is used when the numbers are positive. Not 0 or negative.

yeo jhonson : 
    
    yeo and jhonson are two datascientists collaberatede and give this method. 
    This method fixes the limitations of box cox method i.e. to work on numbers which are 0 or less than 0 

    You will find about it more, just check the respective code file




