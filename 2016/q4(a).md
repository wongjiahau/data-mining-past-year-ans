## (i)
- K-Fold
    - In this  method, we will separate the data into K-number of folds(AKA portion).
    - For example, if we use K=3, then we will separate the data equally (and randomly) into 3 parts, let say we name it part A, part B, and part C.
    - Then in the first iteration, we use AB as training data and C as test data.
    - In 2nd iteration, BC as training data, A as test data.
    - In 3rd iteration, AC as training data, B as test data.
    - The figure below use K=4.
    - ![image](https://user-images.githubusercontent.com/23183656/39743484-95c9f392-52d3-11e8-9515-90c231f030d2.png)
- Hold-out
    - This method is the most simple method, where we simply define how many percent of the data we want to set as training data and testing data.
    - Usually, we will set 70% as training data and 30% as testing data
    - Of course, we need to use a random picker to randomly take out 70% of the data as training data and the remaining will be the testing data
- Leave-one-out
    - This is similar as the K-fold method, however, you only take ONE record as testing data for each iteration.
    - For example, if you only have 10 records of data, then you need to iterate 10 times for training.
    - In the first iteration, you use the first record as testing data, and the other 9 record as training data.
    - Then you repeat the step above until every record had become a testing data before.

## (ii)
We use Leave-one-out method instead of K-Fold when we have very limited amount of data.   

For example, we have only 10 pictures of fruits, and we want to train the classifier to classify the photos, we will need to apply the Leave-one-out method.  

However, if we have few thousands or millions of data, we will need to apply K-fold, if we use Leave-one-out the training will take too long.

## (iii)
Holdout
- Pros 
    - Fully independent data; only needs to be run once so has lower computational costs.
- Cons
    - Performance evaluation is subject to higher variance given the smaller size of the data.

K-Fold
- Pros
    - Prone to less variation because it uses the entire training set.
- Cons
    - Higher computational costs; the model needs to be trained K times at the validation step (plus one more at the test step).