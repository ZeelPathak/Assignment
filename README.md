Files used from this dataset:
1. features.txt - includes the descriptions for features measured
2. train/X_train.txt - includes the measurements of the features in train set (one row - 1 measurement of 561 features)
3. test/X_test.txt - includes the measurements of the features in test set
4. train/subject_train.txt - subject for each measurement from the train set
5. test/subject_test.txt - subject for each measurement from the test set
6. train/y_train.txt - activity for each measurement from the train set
7. test/y_test.txt - activity for each measurement from the test set


download.file - Downloads the data



unzip - unzips the files from the downloaded data



Next step is to read the train tables, test tables, features vector and activity lables 



After reading we assign the column names to train tables, test tables and activity lables for clear understanding


We then merge  the columns of test and train tables by using cbind() which results in mrg_train and mrg_test, using rbind() we combine mrg_train and mrg_test and store in srtALLInOne data frame


After merging, we extract only the measurements on the mean and standard deviation for each measurement


we read the column names in the data frame


Create vector for defining ID, mean and standard deviation


Using descriptive activity names to name the activities in the data set


Creating tidy data with the mean of each variable for each activity and each subject and order the same


And the last step is writing the tidy data in txt file
