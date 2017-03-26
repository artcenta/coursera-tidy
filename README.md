# Getting and Cleaning Data - Project

Source dataset https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.

You should create one R script called run_analysis.R that does the following.
1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive activity names.
5. Creates a second, independent tidy data set with the average of each variable for each activity and each subject.

# Notes
+ Only variables containing mean() & std() are used.
+ Download the zip file from the source, if not exists
+ Unzip the file, if not exists directory "UCI HAR Dataset"

Constructed using the following:


> R.version
--
platform       x86_64-w64-mingw32          
arch           x86_64                      
os             mingw32                     
system         x86_64, mingw32             
status                                     
major          3                           
minor          3.2                         
year           2016                        
month          10                          
day            31                          
svn rev        71607                       
language       R                           
version.string R version 3.3.2 (2016-10-31)
nickname       Sincere Pumpkin Patch       

# Running

$ Rscript run_analysis.R

# Execution Log

-- Loading UCI HAR Dataset...
-- UCI HAR Dataset
-- [1] "activity_labels.txt" "features.txt"        "features_info.txt"   "README.txt"         [5] "test"                "train" 
-- Loading activity_labels.txt...
-- Loading features.txt...
-- Loading the test set...
-- UCI HAR Dataset/test
--[1] "Inertial Signals" "subject_test.txt" "X_test.txt"       "y_test.txt"
-- Loading subject_test.txt...
-- Loading X_test.txt...
-- Loading Y_test.txt...
-- Building test set...
-- Loading the training set...
-- UCI HAR Dataset/train
-- [1] "Inertial Signals"  "subject_train.txt" "X_train.txt"       "y_train.txt"    
-- Loading subject_train.txt...
-- Loading X_train.txt...
-- Loading Y_train.txt...
-- Building training set...
-- Merging the training and the test sets to create one data set...
-- Extracting only the measurements on the mean and standard deviation for each measurement...
-- Using descriptive activity names to name the activities in the data set...
-- Labelling the data set with descriptive activity names...
-- Building a second, independent tidy data set with the average of each variable for each activity and each subject...
-- Writing tidy.mean.txt ...
-- Writing tidy.txt ...


# Yields 
tidy.txt & tidy.mean.txt.