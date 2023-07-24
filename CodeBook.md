# Codebook for Human Activity Recognition Using Smartphones Dataset

This codebook describes the variables, the data, and the transformations performed to clean up the data.

## 1. Source Data

The data used in this project represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

The data for the project are available here:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

## 2. Dataset Information

The experiments were carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, 3-axial linear acceleration and 3-axial angular velocity were captured at a constant rate of 50Hz.

The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

## 3. Variables

- `subject`: An identifier of the subject who carried out the experiment. Its range is from 1 to 30.

- `activity`: Activity performed by the subject. It is a factor with 6 levels: 

    - WALKING
    - WALKING_UPSTAIRS
    - WALKING_DOWNSTAIRS
    - SITTING
    - STANDING
    - LAYING

- Other variables represent mean and standard deviation measurements from the accelerometer and gyroscope. They are as follows:

    - Variables starting with 'timeDomain' indicate time domain signals.
    - Variables starting with 'frequencyDomain' indicate frequency domain signals.
    - 'Accelerometer' in variable names indicates acceleration signal.
    - 'Gyroscope' in variable names indicates gyroscope signal.
    - 'Body' in variable names indicates body motion components.
    - 'Gravity' in variable names indicates gravity motion components.
    - 'Jerk' in variable names indicates jerk signals.
    - 'Magnitude' in variable names indicates magnitude of the signals calculated using the Euclidean norm.
    - 'Mean' in variable names indicates mean value of the signals.
    - 'StandardDeviation' in variable names indicates standard deviation of the signals.

All the values are unit-less because they were normalized and bounded within [-1, 1] during the preprocessing of the raw data.

## 4. Transformations

The raw data were processed by the R script to create a tidy dataset with the average of each variable for each activity and each subject. The steps included merging the training and the test datasets, extracting the measurements on the mean and standard deviation for each measurement, adding descriptive activity names, and creating a second, independent tidy dataset with the average of each variable for each activity and each subject.

---

You can further expand this codebook by providing more details about each of the variables, explaining the units of measurement, and giving additional information about the transformations done on the raw data.