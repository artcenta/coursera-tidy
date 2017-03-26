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

1. Loading UCI HAR Dataset...
2. UCI HAR Dataset
3. [1] "activity_labels.txt" "features.txt"        "features_info.txt"   "README.txt"         [5] "test"                "train" 
4. Loading activity_labels.txt...
5. Loading features.txt...
6. Loading the test set...
7. UCI HAR Dataset/test
  *[1] "Inertial Signals" "subject_test.txt" "X_test.txt"       "y_test.txt"
8. Loading subject_test.txt...
9. Loading X_test.txt...
10. Loading Y_test.txt...
11. Building test set...
12. Loading the training set...
13. UCI HAR Dataset/train
  * [1] "Inertial Signals"  "subject_train.txt" "X_train.txt"       "y_train.txt"    
14. Loading subject_train.txt...
15. Loading X_train.txt...
16. Loading Y_train.txt...
17. Building training set...
18. Merging the training and the test sets to create one data set...
19. Extracting only the measurements on the mean and standard deviation for each measurement...
20. Using descriptive activity names to name the activities in the data set...
21. Labelling the data set with descriptive activity names...
22. Building a second, independent tidy data set with the average of each variable for each activity and each subject...
23. Writing tidy.mean.txt ...
24. Writing tidy.txt ...


# Yields 
tidy.txt & tidy.mean.txt.