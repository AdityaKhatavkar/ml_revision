# ml_revision

Hello! I am keeping track of concepts i will revised over the course of practice sessions

24/ 1 / 2025
I worked on california house pricing dataset. Just a mini project makes the concepts more stronger. Visualizing the dataset, data preprocessing and transformation. I got r2_score of about 0.62 . I will make valid modifications in the code that will incresase the r2_score. I placed this file in the folder : regularization/elastic_net/housige_price.ipynb

22/1/2025
Today i saw the underlying math of lasso regression. How it creates sparsity in the dataset. Effects of L1 norm/ L1 penelty in lasso regression. How it forms diamond-shaped sharp corner, it is different from the smooth curver form by the L2 penalty of ridge regression.
Elastic regression is another method which is combination of ridge and lasson regression. It is pretty efficient when large dataset is available. On this knowledge i  am making a model that will predict the median_prices house using the house_price_california dataset. In the upcoming days i will done with it. Thank you!

21/1/2025
Revision was about the concepts of regularization. I implented the code for n_dimensional ridge regression. I compare the results of prebuilt ridge regression from sklearn and the class that i coded from scratch. Moreover i revise the lasso regression concept (theory, sklear_implementation). For more detail about code, check the respective .ipynb files.

20/1/2025
Although i didnt commit to the repo for coupl of days back. But i was in touch with the stuff of machine larning. I completed the some part which was left related to the PCA. I perform the PCA on the MNIST digit dataset. I used it for visualization of the dataset by converting it into lower dimensions. Then i  saw the basic concept of ridge rgression like why it is used? , advantages , disadvantages. Moreover its mathematical imputation make the idea more clear. I saw the the difference between the results of prebuilt ridge regression from sklearn and the class that i coded from scratch. Have a look on the respective .ipynb files. Thank you!

15/1/2025
PCA is a technique which is use to reduce the dimensions of the data with keeping the essence of the data.
I saw the theory, problem formulation, prerequisites for the concept, its geometric intution, mathematical formulation, code. Check the readme and code file for the same. This time i use to create rough handy-notes becoz it was getting difficult to express it in digital files. It is wiritten in english + marathi (my mother toung). 

14/1/2025
Today i saw concepts related to handeling mix variables, dealing with data and time columns, feature construction and curse of dimensionality.
We can seperate the numerical part and the categorical part present in the same column or in same cell (i.e. mix_data) with the help of pandas. This action can improve the performance of the model as it gets easy to deal with such sorted data.
We can get insights from the date and time columns also. Like year, month, day, hour, minute, etc.
Feature construction will make the data more clearer and easy for model to understand it.
Lastly i saw theory about the cusre of dimensionality, need of optimal number of features and how it affects the performance of the model. 
Today i performed the pratical coding exercise on the topics handeling_mix_variable, feature construction. In the upcoming practice session i will performe the code on remaining stuff. Have a look on the code files in the repository. Thank you! :)

13/1/2025
On this day i implemented the techniques of binning. Understood it better with the help of visualization. Observed the difference between before implementing the binning and after implementing binning Code and concept is written in the respective files

11/1/2025
Today is saw the concept about encoding numerical feautures into the categorical features. Code part on it is not done this day. We will complete in next day. 

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





