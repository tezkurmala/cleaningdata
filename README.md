run_analysis
============

Load features to assign the column names to training and test data
~~~
features <- read.table("UCI HAR Dataset\\features.txt", stringsAsFactors=FALSE)
~~~
Load training observations
~~~
xtrain <- read.table("UCI HAR Dataset\\train\\X_train.txt")
~~~
Change the column names and set to features loaded
~~~
colnames(xtrain)<-features$V2
~~~
Load activity that corresponds to each observation in training data (with column name as 'Activity')
~~~
ytrain <- read.table("UCI HAR Dataset\\train\\y_train.txt", col.names = c("Activity"))
~~~
Load subject that corresponds to each observation in training data (with column name as 'Subject')
~~~
subjecttrain <- read.table("UCI HAR Dataset\\train\\subject_train.txt", col.names = c("Subject"))
~~~
Form Combined Training Data by merging columns in order of Subject, Activity, Observations
~~~
train <- cbind(subjecttrain, ytrain, xtrain)
~~~
Load test observations
~~~
xtest <- read.table("UCI HAR Dataset\\test\\X_test.txt")
~~~
Change the column names and set to features loaded
~~~
colnames(xtest)<-features$V2
~~~
Load activity that corresponds to each observation in test data (with column name as 'Activity')
~~~
ytest <- read.table("UCI HAR Dataset\\test\\y_test.txt", col.names = c("Activity"))
~~~
Load subject that corresponds to each observation in test data (with column name as 'Subject')
~~~
subjecttest <- read.table("UCI HAR Dataset\\test\\subject_test.txt", col.names = c("Subject"))
~~~
Form Combined Test Data by merging columns in order of Subject, Activity, Observations
~~~
test <- cbind(subjecttest, ytest, xtest)
~~~
Merge the rows of Combine Training Data and Combined Test Data to form complete data frame
~~~
mergedData <- rbind(train, test)
~~~
Create a subset that carries information about Subject, Activity, Mean, Standard Deviation
~~~
mergedDataWithMeansAndStd <- mergedData[ , grepl( "Subject|Activity|-std\\(\\)|-mean\\(\\)" , names( mergedData ) ) ]
~~~
Replace Activity Numbers by corresponding Activity Labels
Load Activity Labels
~~~
activities <- read.table("UCI HAR Dataset\\activity_labels.txt", stringsAsFactors=FALSE)
~~~
Apply the replacements thought out each observation in the merged data
~~~
for(i in 1:nrow(activities)){
  mergedDataWithMeansAndStd$Activity[mergedDataWithMeansAndStd$Activity == activities$V1[i]] <- activities$V2[i]
}
~~~
Rename columns of merged/subset data to user-friendly column names
~~~
colnames(mergedDataWithMeansAndStd) <- gsub("-std\\(\\)","StandardDeviation",colnames(mergedDataWithMeansAndStd))
colnames(mergedDataWithMeansAndStd) <- gsub("-mean\\(\\)","Mean",colnames(mergedDataWithMeansAndStd))
colnames(mergedDataWithMeansAndStd) <- gsub("^t","time",colnames(mergedDataWithMeansAndStd))
colnames(mergedDataWithMeansAndStd) <- gsub("^f","frequency",colnames(mergedDataWithMeansAndStd))
colnames(mergedDataWithMeansAndStd) <- gsub("Acc","Accelerometer",colnames(mergedDataWithMeansAndStd))
colnames(mergedDataWithMeansAndStd) <- gsub("Gyro","Gyroscope",colnames(mergedDataWithMeansAndStd))
colnames(mergedDataWithMeansAndStd) <- gsub("Mag","Magnitude",colnames(mergedDataWithMeansAndStd))
colnames(mergedDataWithMeansAndStd) <- gsub("-","Of",colnames(mergedDataWithMeansAndStd))
~~~
Find the average of every column when grouped by each Subject and each Activity
~~~
library(reshape2)
molten <- melt(mergedDataWithMeansAndStd, id = c("Subject", "Activity"))
averagesOfMergedDataWithMeansAndStd <- dcast(molten, Subject + Activity ~ variable, mean)
~~~
Store to a file and display the result
~~~
write.table(mergedDataWithMeansAndStd, file = "tidyDataAveraged.txt", row.names = FALSE)
print(mergedDataWithMeansAndStd)
~~~