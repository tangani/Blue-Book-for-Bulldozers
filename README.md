Predicting bulldozer prize using Machine Learning
This is a time series project whose purpose is to predict the sale price of a bulldozer.

1.Problem definition
How well can the model predict the future sale price of a bulldozer given a set of characteristics and previous examples of similar bulldozers sale.

2. Data description
The data contained here was obtained from Kaggle https://www.kaggle.com/c/bluebook-for-bulldozers/data

The data for this competition is split into three parts:

Train.csv is the training set, which contains data through the end of 2011.
Valid.csv is the validation set, which contains data from January 1, 2012 - April 30, 2012 You make predictions on this set throughout the majority of the competition. Your score on this set is used to create the public leaderboard.
Test.csv is the test set, which won't be released until the last week of the competition. It contains data from May 1, 2012 - November 2012. Your score on the test set determines your final rank for the competition.
The key fields are in train.csv are:

SalesID: the uniue identifier of the sale MachineID: the unique identifier of a machine. A machine can be sold multiple times saleprice: what the machine sold for at auction (only provided in train.csv) saledate: the date of the sale

There are several fields towards the end of the file on the different options a machine can have. The descriptions all start with "machine configuration" in the data dictionary. Some product types do not have a particular option, so all the records for that option variable will be null for that product type. Also, some sources do not provide good option and/or hours data.

3. Evaluation
The evaluation metric is the RMSLE(root mean squared log error) between the actual and predicted auction prices.

Note: The goal for most regression evaluation metrics is to minimize the error.My goal for this project is to minimize the RMSLE.

4. Features
The features of this data are given in detail in the data dictionary on kaggle https://www.kaggle.com/c/bluebook-for-bulldozers/data