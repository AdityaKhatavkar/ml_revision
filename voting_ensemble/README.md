

# What is Voting ensemble learning?
     
     A technique that uses multiple ml models, and the final answer is either mode  or mean of  all individual predictions/ classifications.



# Some assumptions for Voting ensemble learning:

    - Individual models should be independent of each other.
    - Minimum accuraccy of each model should be 50%.


# Soft voting Vs Hard voting 

    By default, sklearn is having hard voting.


    * Hard Voting : 
        - Each classifier votes for a single class prediction
        - Final prediction is determined by majority vote (most frequently predicted class)


    * Soft Voting :
        -Instead of single class predictions, classifiers output probability distributions
        -Final prediction is based on averaged probability scores across all classifiers
        -More nuanced approach that considers confidence of each classifier 
        

    * Key Difference:
        Hard voting counts votes, while soft voting averages probability predictions, making soft voting generally more sophisticated and potentially more accurate.