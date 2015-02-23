# CodeBook

This CodeBook describes the data, variables and transformations that occur in the script.

# Data 
1. Source of Data: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
2. Raw Data: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

## The dataset includes the following files:

* 'README.txt'
* 'features_info.txt': Shows information about the variables used on the feature vector.
* 'features.txt': List of all features.
* 'activity_labels.txt': Links the class labels with their activity name.
* 'train/X_train.txt': Training set.
* 'train/y_train.txt': Training labels.
* 'test/X_test.txt': Test set.
* 'test/y_test.txt': Test labels.
* 'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample 
* 'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'
* 'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration.
* 'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second.

## Transformation:

1. The script requires plyr library.
2. The run_analysis script:

* Reads the training and test data sets
* Merges the training and test data sets into one data set (vector: subject_data)
* Extracts  the measurements on the mean and standard deviation for each measurement
* Uses simple/descriptive activity names and label appropriately
* Creates independent tidy data set with the average of each variable
* Writes new tidy averages data into a text file

