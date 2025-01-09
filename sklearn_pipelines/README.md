Pipelines in sklearn are not any algorithm but a technique to combine multiple steps. Such that output of one step is input to the next step. Pipelines useful in making production level codes.

Syntax : class sklearn.pipeline.Pipeline(steps, *,  memory=None, verbose=False)

steps : List of tuples, each tuple contain name of the tranformation followed by actual transformation. 
        for eg: steps = [('scaler', StandardScaler()), ('model', LogisticRegression())]

memory : Location to store the cache of the pipeline. Default is None.
         Use to reduce do repetative transformaitons which is not necessary.
         for eg.
          We have to fit the pipeline multiple time. And the pipe contain transformation of standartscaler.
          After one fit, output of standard scaler will be cached and will be used for the next fit.
          So the repetation of same work and the time is reduced. 
          You will get to know about it in the code snippet.

verbose : If true, the time elapsed while fitting the pipeline is printed.  

In previouse versions pipelines used to support the parameter called as 'transform_input'.This parameter specifies the names of metadata parameters (other than X) that should go through the pipeline and be transformed.
But now it is removed

Link fo the sklearn doc : https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html