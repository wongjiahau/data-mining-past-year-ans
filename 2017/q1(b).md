## (i)
- Supervised machine learning
- It is method used to classify data when the input data is labelled, in this case, since all faces is labelled (I assumed that), we can train the computer to recognize them using some classifier algorithm
- Examples are:
    - Multilayer perceptron
    - Deep Convolutional Network

## (ii)
- First, he need to partition the data into testing and training data. Usually we use 30% of the data for testing while 70% of the data for training
- Then, we train the model using the training data, in Scikit learn, we will call the `.fit()` method.
- After that, we predict the result using the trained model
- Lastly, we measure the performance of the model by using some metric calculation (e.g. Confusion Matrix, accuracy, precision etc.)
- Then, we repeat from step 2, but this time we will tune the parameters of the model
- Keep on repeating this process until the accuracy reach the desired level