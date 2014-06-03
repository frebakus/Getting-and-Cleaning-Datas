This program creates data frames for train data and test data. Then merges them to create a tidy data set. Extracts only the measurements on the mean and standard deviation for each measurement. Uses descriptive activity names to name the activities in the data set Appropriately labels the data set with descriptive activity names. Creates a second, independent tidy data set with the average of each variable for each activity and each subject. The location of this R program is at the root folder(UCI HAR Dataset) of the extracted zip file

Different steps followed in this program are: 1. Read the file features.txt in table format and created a data frame named features
1.Read the file subject_train.txt in table format (read.table function) to create a data frame subjectTrain also read the file X_train.txt in table fomat and creates a data frame named XTrain also read the file y_train.txt in table fomat and creates a data frame named yTrain
2.create the trainData using column bind for the data frames subjectTrain,yTrain and XTrain using cbind function
3.Read the file subject_test.txt in table format (read.table function) to create a data frame subjectTest also read the file X_train.txt in table fomat and creates a data frame named XTest also read the file y_train.txt in table fomat and creates a data frame named yTest

4.create the testData using column bind for the data frames subjectTest,yTest and XTest


5.create a consolidated data frame 'data' from the data frames trainData and testData using the rbind function

6.arrange the consolidated data frame 'data' by "id" field
7.Uses descriptive activity names to name the activities in the data set.
8.Appropriately label the data set with descriptive activity names. 10.Extract only the measurements on the mean and standard deviation for each measurement.
9.create a results folder
10.save the tidy data set into the results folder
11.Create a second, independent tidy data set with the average of each variable for each activity and each subject.
12.Add "_mean" to colnames
13.Save tidy dataset2 into results folder
