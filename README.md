# Module 13 Assignment 

This assignment is to predict whether Alphabet Soup funding applicant will be successful if funded by Alphabet Soup.

The first thing to do is preparing data in a correct format for model training and testing. I split the data by X and y. y is the output variable to predict if applicant will be successful. Also, this is a balanced data according to the value count of y variable. X is dummary variable for feature input variable to be further used for model testing. After X and y variable being setup, I use train_test_split function to split 75% of training data, 25% of data for testing by default. Then I can scale them by normalizing it to Z-score. 

After data are prepared, I used 3 different methods to train and test my data under Sequential model. 

1. I set up 2 hidden layers with relu functions, output with Tanh function, fit and run the training data with model by 50 epochs. The accuracy in last run is 73.48%, loss is 55.23%. Base on this accuracy and loss percentage, this model is not doing well. I need to find another solution to improve accuracy.

2. For alternative model 1, I add regularization, increase the numbers of first and second hidden layer, output layer use sigmoid function, then fit the training data, run the model with 100 epochs. The accuracy is 74.04%, loss is 53.56%. Both percentages have slight improvement, but it is still not enough. I need to create another model to see if it will run better.

3. For alternative model 2, I add third layer, fit the traning data and run the model with 150 epochs, the accuracy is 74.51%, loss is 52.35%, which also only have a slight improvement. 

Overall, Sequential model with these 3 scenario are not performing well, accuracy are lower than 80% and loss are above 50%. Even though I evaluate with test data, there is not much difference. 

