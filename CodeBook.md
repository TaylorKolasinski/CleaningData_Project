# Code Book

This code book summarizes the resulting data fields in clean_and_tidy.txt as well as the 5 steps that were taken to clean the data.

# Steps
The following steps occur in run_anaylsis.R to produce the final clean dataset.

1) We create one dataset by merging the training and test sets from the following files:
  * `features.txt`
  * `subject_test.txt`
  * `activity_labels.txt`
  * `subject_train.txt`
  * `x_test.txt`
  * `x_test.txt`
  * `x_train.txt`
  * `y_train.txt`

2) Calculate and extract the measurements for the mean and standard deviation.

3) Rename the activites with their descriptive names by marging with the activityType table.

4) Relabel the the data set with the descripting activity names.

5) Create a new tidy data set with the avaerages of each variable for the subjects and activity.

## Identifiers

* `subject` - The ID of the test subject
* `activity` - The type of activity performed when the corresponding measurements were taken

## Measurements

* `tBodyAccMeanX`
* `tBodyAccMeanY`
* `tBodyAccMeanZ`
* `tBodyAccStdX`
* `tBodyAccStdY`
* `tBodyAccStdZ`
* `tGravityAccMeanX`
* `tGravityAccMeanY`
* `tGravityAccMeanZ`
* `tGravityAccStdX`
* `tGravityAccStdY`
* `tGravityAccStdZ`
* `tBodyAccJerkMeanX`
* `tBodyAccJerkMeanY`
* `tBodyAccJerkMeanZ`
* `tBodyAccJerkStdX`
* `tBodyAccJerkStdY`
* `tBodyAccJerkStdZ`
* `tBodyGyroMeanX`
* `tBodyGyroMeanY`
* `tBodyGyroMeanZ`
* `tBodyGyroStdX`
* `tBodyGyroStdY`
* `tBodyGyroStdZ`
* `tBodyGyroJerkMeanX`
* `tBodyGyroJerkMeanY`
* `tBodyGyroJerkMeanZ`
* `tBodyGyroJerkStdX`
* `tBodyGyroJerkStdY`
* `tBodyGyroJerkStdZ`
* `tBodyAccMagMean`
* `tBodyAccMagStd`
* `tGravityAccMagMean`
* `tGravityAccMagStd`
* `tBodyAccJerkMagMean`
* `tBodyAccJerkMagStd`
* `tBodyGyroMagMean`
* `tBodyGyroMagStd`
* `tBodyGyroJerkMagMean`
* `tBodyGyroJerkMagStd`
* `fBodyAccMeanX`
* `fBodyAccMeanY`
* `fBodyAccMeanZ`
* `fBodyAccStdX`
* `fBodyAccStdY`
* `fBodyAccStdZ`
* `fBodyAccMeanFreqX`
* `fBodyAccMeanFreqY`
* `fBodyAccMeanFreqZ`
* `fBodyAccJerkMeanX`
* `fBodyAccJerkMeanY`
* `fBodyAccJerkMeanZ`
* `fBodyAccJerkStdX`
* `fBodyAccJerkStdY`
* `fBodyAccJerkStdZ`
* `fBodyAccJerkMeanFreqX`
* `fBodyAccJerkMeanFreqY`
* `fBodyAccJerkMeanFreqZ`
* `fBodyGyroMeanX`
* `fBodyGyroMeanY`
* `fBodyGyroMeanZ`
* `fBodyGyroStdX`
* `fBodyGyroStdY`
* `fBodyGyroStdZ`
* `fBodyGyroMeanFreqX`
* `fBodyGyroMeanFreqY`
* `fBodyGyroMeanFreqZ`
* `fBodyAccMagMean`
* `fBodyAccMagStd`
* `fBodyAccMagMeanFreq`
* `fBodyBodyAccJerkMagMean`
* `fBodyBodyAccJerkMagStd`
* `fBodyBodyAccJerkMagMeanFreq`
* `fBodyBodyGyroMagMean`
* `fBodyBodyGyroMagStd`
* `fBodyBodyGyroMagMeanFreq`
* `fBodyBodyGyroJerkMagMean`
* `fBodyBodyGyroJerkMagStd`
* `fBodyBodyGyroJerkMagMeanFreq`

## Activity Labels

* `WALKING` (value `1`): subject was walking during the test
* `WALKING_UPSTAIRS` (value `2`): subject was walking up a staircase during the test
* `WALKING_DOWNSTAIRS` (value `3`): subject was walking down a staircase during the test
* `SITTING` (value `4`): subject was sitting during the test
* `STANDING` (value `5`): subject was standing during the test
* `LAYING` (value `6`): subject was laying down during the test
