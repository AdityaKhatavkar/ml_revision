# ml_revision

Hello! I am keeping track of concepts i will revised over the course of practice sessions

10/ 1/ 2025
 Normal distribution of data helps to train models efficiently (specially linear models). If data is not normally distributed, we can apply transormation on it to make it better. Some examples of mathematical transformations are: log(x), sqrt(x), reciprocal, power, boxcox, yeo johson. Today i explore the tranformation techniques. I deeply analyze the impact of it on the model training. Visualizing the PDA of features before and after the transformation makes the  concept more clear. Come check this out. 

date 9/1/2025
On this day i revised the concept of pipelines in sklearn. Pipelines in sklearn are not any algorithm but a technique to combine multiple steps. Such that output of one step is input to the next step. Pipelines useful in making production level codes. Pipleines support parameters like steps, memory, verbose, etc. The code and the notes are written in the respective file. Do check it out :)

date 7/1/2024
Conversion of categorical features to numerical features is important factor. Categorical column can be of two types viz. nominal and ordinal. According to the type of categorical feature we have to select best suiting encoding technique. In this notebook i practice concept of label_encoding-ordinal_encoding, one hot encoding (its varients like frequency encoding , k-1 encoding), column_transformer from sklearn. Revise about what is dummy variable trap and how to handle it. Related code and the notes are written in respective files.

date 29/12/2024
Outliers can affet the performance of ml algorithms. There are some ways to deal with outliers. Methods like trimming, capping, z_score, boxplot and iqr, percentile winzarization are useful for the same. Today I revised these concepts. Code and explanation is written in the respective files.

date 28/12/2024
KNN imputation is one of the method use in multivariate imputation. We can implement it using sklearn.impute module(from sklearn.impute import KNNImputer). I revised the concept from online sources. Next i implemented the code. Tunning the values of 'n_neighbour' and opting weight = 'distance' gave better results. Check the code for the same.

date 27/12/2024
On this day in continuation with the revision of 'Handelling missing values' i brush up my knowledge regarding mean/median imputation, random imputation, arbitary value imputation, end of distribution imputation. I observed the data pattern before and after the operation on missing values in the dataset. Moreover i plotted some graph about it to analyzed it more clearly. Code and concept is written in the respective files. Thank you!





