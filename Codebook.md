---
title: "Codebook"
author: "hbapuram"
date: "6/26/2020"
output: html_document
---

# Codebook

The `run_analysis.R` script performs the data preparation and then followed by the 5 steps required as described in the course project’s definition.

  1. **Download the dataset** 
      * Dataset downloaded and extracted under the folder called `UCI HAR Dataset`
      
  2. **Assign each data to variables** 
      * `features` <- `features.txt` : 561 rows, 2 columns
      
        *The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ.*

      * `activityLabels` <- `activity_labels.txt` : 6 rows, 2 columns
        
        *List of activities performed when the corresponding measurements were taken and its codes (labels)*
        
      * `subject_test` <- `test/subject_test.txt` : 2947 rows, 1 column

        *Contains test data of 9/30 volunteer test subjects being observed*

      * `xtest` <- `test/X_test.txt` : 2947 rows, 561 columns

        *Contains recorded features test data*

      * `ytest` <- `test/y_test.txt` : 2947 rows, 1 columns

        *Contains test data of activities’code labels*

      * `subject_train` <- `test/subject_train.txt` : 7352 rows, 1 column

        *Contains train data of 21/30 volunteer subjects being observed*

      * `xtrain` <- `test/X_train.txt` : 7352 rows, 561 columns

        *Contains recorded features train data*
        
      * `ytrain` <- `test/y_train.txt` : 7352 rows, 1 columns
      
        *Contains train data of activities’code labels*
        
  3. **Merging the train and test data**   
      * `mrg_train` <- created by merging `xtrain` and `ytrain` using **cbind()** function
      
      * `mrg_test` <- created by merging `xtest` and `ytest` using **cbind()** function
      
  4. **Final edited tidy dataset**
      * `tidydata.txt`
      
      
    
