# Run Analysis 
The R script takes the path for the UTC HAR dataset
It then imports the important txt files from the path viz., features and what the various activities are.
The needed features are extracted which are basically the ones with mean or standard deviation through regular expressions.
It then imports the train dataset and then the train labels of activities of the required features whose names were extracted in the previous step.
Same is done for the test data
It then combines the train and test data into one dataset
Since the mean of each of the column is needed. The dataset is grouped according to subject and activity and the aggregate is calculated for each column and recasted into a datafram
The last line of the code saves the data frame into a txt file named 'tidydata.txt.
