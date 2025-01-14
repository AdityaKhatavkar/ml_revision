# What is mixed data: 

    Data is combination of numerical and categorical data.


# How to handle it.

    There can be two types of mixed data occur generally.

    1. Number and letters in the same name. 

    For eg. boogies is railway like b5, b6, s1, s2, a1, a3  
    Here we can split into two columns like with categories b, a, s, and other column with categories. 1,2,3,4,5,

                    (Railway_boogies [s1,s2,a4,a5])---->(Railway_boogies_numerical [1,3,4,5,2])
                            |
                            |
                            |
                (Railway_boogies_categorical [a,s] )


    2. At some places numerical and at some places categorical
    
    Here some places will contain numbers while some places in the column will contain categorical values.

    We will split in the numeical and categorical columns.
        If value orignal column is numrical, it will fall in updated numeical column and categorical column will contain null/nan for that row.
        And vice versa.

# Note : 

    This is to be done with pandas and numpy only becoz sklearn does not provides any feature for this purpose.

Follow the ipynb file for more details regarding coding part. See you there :)