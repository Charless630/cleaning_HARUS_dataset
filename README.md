# getting_and_cleaning_data

This repository contains the R script run_analysis.R that performs an analysis on human activity recognition data. The data is collected from the accelerometers of the Samsung Galaxy S smartphone worn by 30 subjects performing six different activities. The raw data is processed into a clean, tidy dataset containing the average of each measurement for each activity and each subject.

The analysis follows these steps:

Downloading and reading the data: The data is downloaded from the URL and unzipped if it hasn't been already. The training and testing data, along with feature and activity information, are then read into R.

Merging the data: The training and testing datasets are merged into one complete dataset.

Extracting measurements: Only the measurements on the mean and standard deviation for each measurement are extracted from the dataset.

Adding descriptive activity names: The activity identifiers are replaced with descriptive activity names.

Labeling the dataset: The dataset is labeled with descriptive variable names.

Creating a second, tidy dataset: A second, independent tidy dataset is created with the average of each variable for each activity and each subject. This dataset is then written to a text file.
