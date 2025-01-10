cross_val_score: 

syntax : 
sklearn.model_selection.cross_val_score(estimator, X, y=None, *, groups=None, scoring=None, cv=None, n_jobs=None, verbose=0, params=None, pre_dispatch='2*n_jobs', error_score=nan)
Evaluate a score by cross-validation.



estimator : fuction. The object to use to fit the data.


x : independent variables / input features

y : dependent variable / target feature


Returns:
scores
ndarray of float of shape=(len(list(cv)),)
Array of scores of the estimator for each run of the cross validation.