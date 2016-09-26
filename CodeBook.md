This document describes the code inside run_analysis.R.

# Data URL to download
  dataURL

# Local data file
  dataFileZIP

# Directory where data is downloaded
  dirFile
  
# filename (txt or csv) of the clean/tidy data:
  tidyDataFile.txt

# filename (.txt) of the clean/tidy data
  tidyDataFileAVGtxt
  
Steps:
# Download the dataset (. ZIP), which does not exist

# Uncompress data file
 

1. Merge the training and the test sets to create one data set:
 # Combines data table (train vs test) by rows
 
2. Extracts only the measurements on the mean and standard deviation for each measurement:
 # Read features labels
 # Friendly names to features column
 # Search for matches to argument mean or standard deviation (sd)  within each element of character vector
 # Replaces all matches of a string features 

3. Uses descriptive activity names to name the activities in the data set:

4. Appropriately labels the data set with descriptive activity names:
 # Read activity labels
 # Combines data table by columns
  
5. Creates a 2nd, independent tidy data set with the average of each variable for each activity and each subject:
  # Activity and Subject name of columns 
  # Created csv (tidy data set) in diretory
  # Created csv (tidy data set AVG) in diretory
  # write.csv(tidyDataAVGSet, tidyDataFileAVG)
  # Create txt (tidy data set AVG) in diretory
  