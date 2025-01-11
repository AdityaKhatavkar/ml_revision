# When we do encoding of numerical values/features.
        suppose you have dataset about downloads of apps from the playstore.
        some apps will have very less downloads while some of them will have insanely large number of downloads.
        In that case we can make the categories like downloads < 100, < 1k , < 10K , < 100k , < 1 M , etc.
        It will become easy to handle it

# There are two techniques for it

        1) Discritization / Binning
        2) Binarization


# Discritization / Binning

        Process of transforming continuous variables into discrete variables by createing a set of contiguous intervals that span the range of the variable's value. Discritization also called as binning, where bin is an alternative name for the interval.

        हिस्ट प्लॉट मध्ये कसे intervals तयार होतात त्या प्रमाणे.  


# Why use Binnig.

        1> To handle Outliers
        2> To improve the value spread.


# Types of binning 

        1> Unsupervised binning --------------> Equal width binning, Equal frequencey binning,  K means binning
        2> Supervised ------------------------> Decision tree binning
        3> Custom binning 


# Equal widht binning (Uniform binning):
         
         We decide number of bins

         Formula :- (max - min)/bins

         For eg: 0,1,2,3,........., 100
                 I want 10 bins
                 Hence (100 - 0)/10, size of bins will be equal to 10
                 0-10, 10-20, 20-30, 30-40

        Advantages: 
                Good in handeling outliers
                No change in spread of data


# Equal frequency (quantile) binning:

        Suppose i want 10 intervals.
        Then each interval will contain 10% of the total observations.

        Advantages :
                Good in handeling outliers
                Effectively changes the spread of the data.
                Make the value spread uniform.

        It is usally used more than uniform. Sklearn has also this is as default method.


# K means binning: 

        When the distribution of the data is in the form of clusters. Then we use this strategy. 
        Here we simply apply the k means algorithm on the dataset and then we create the intervals.