---
title: "codeBook.md"
author: "Paul Roetman"
date: "15 June 2017"
output: html_document
---

## Code Book

### Data

The data in the results.txt file is derived from the test and training data files supplied within the "UCI HAR Dataset.zip" file. There are two modes for the data, a test mode and a train mode. The data structures within each mode are identical, the only difference is the volume of data.

#### X_{mode}.txt

Each of the test and train directories contains an X file that contains the raw data for the from the measurements from the smartphone.

#### Y_{mode}.txt

This file contains the activity for each corrosponding line the in X_{mode}.txt file. These activites (numbered 1 through to 6) can be mapped to a physical task using the file activity_labels.txt, for example - activity 1 is "Walking".

#### subject_{mode}.txt

This file contains the subject for each corrosponding line in the X_{mode}.txt file. There are 30 subjects within both test and train data.


#### Features

The features.txt file contains the column headings for the X file data.


### Variables

Below is the list of columns in the result.txt file. Each column that ends in _Mean is the average derived from there respective columns in the train and test data files, with one line each per Subject per Activity.

While the original data contained many more variables, the only data retained for this result set were the variables pertaining to either Mean (Mean) or Standard deviation (STD). Each variable that has any relationship to mean or std has been retained, all others have been removed.

The data from train and the data from test were loaded and concatenated together, then the mean data was extracted per subject per activity. This new data set is written to the file "results.txt".

For each variable, all abbriviations have been removed when comparing to the original data set.

* Subject
        2 
        Range 1-30. Id of the subject for the mean results
        
* Activity
        20 
        LAYING
        SITTING
        STANDING
        WALKING
        WALKING_DOWNSTAIRS
        WALKING_UPSTAIRS
        
* TimeBodyAccelerationMeanX_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationMeanY_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationMeanZ_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationSTDX_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationSTDY_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationSTDZ_Mean
        16
        Range -1 to 1, floating point number
        
* TimeGravityAccelerationMeanX_Mean
        16
        Range -1 to 1, floating point number
        
* TimeGravityAccelerationMeanY_Mean
        16
        Range -1 to 1, floating point number
        
* TimeGravityAccelerationMeanZ_Mean
        16
        Range -1 to 1, floating point number
        
* TimeGravityAccelerationSTDX_Mean
        16
        Range -1 to 1, floating point number
        
* TimeGravityAccelerationSTDY_Mean
        16
        Range -1 to 1, floating point number
        
* TimeGravityAccelerationSTDZ_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationJerkMeanX_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationJerkMeanY_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationJerkMeanZ_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationJerkSTDX_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationJerkSTDY_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationJerkSTDZ_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeMeanX_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeMeanY_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeMeanZ_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeSTDX_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeSTDY_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeSTDZ_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeJerkMeanX_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeJerkMeanY_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeJerkMeanZ_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeJerkSTDX_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeJerkSTDY_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeJerkSTDZ_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationmagnitudeMean_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationmagnitudeSTD_Mean
        16
        Range -1 to 1, floating point number
        
* TimeGravityAccelerationmagnitudeMean_Mean
        16
        Range -1 to 1, floating point number
        
* TimeGravityAccelerationmagnitudeSTD_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationJerkmagnitudeMean_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyAccelerationJerkmagnitudeSTD_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopemagnitudeMean_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopemagnitudeSTD_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeJerkmagnitudeMean_Mean
        16
        Range -1 to 1, floating point number
        
* TimeBodyGyroscopeJerkmagnitudeSTD_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationMeanX_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationMeanY_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationMeanZ_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationSTDX_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationSTDY_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationSTDZ_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationMeanFrequencyX_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationMeanFrequencyY_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationMeanFrequencyZ_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationJerkMeanX_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationJerkMeanY_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationJerkMeanZ_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationJerkSTDX_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationJerkSTDY_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationJerkSTDZ_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationJerkMeanFrequencyX_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationJerkMeanFrequencyY_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationJerkMeanFrequencyZ_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyGyroscopeMeanX_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyGyroscopeMeanY_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyGyroscopeMeanZ_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyGyroscopeSTDX_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyGyroscopeSTDY_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyGyroscopeSTDZ_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyGyroscopeMeanFrequencyX_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyGyroscopeMeanFrequencyY_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyGyroscopeMeanFrequencyZ_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationmagnitudeMean_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationmagnitudeSTD_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencyBodyAccelerationmagnitudeMeanFrequency_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencybodyAccelerationJerkmagnitudeMean_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencybodyAccelerationJerkmagnitudeSTD_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencybodyAccelerationJerkmagnitudeMeanFrequency_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencybodyGyroscopemagnitudeMean_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencybodyGyroscopemagnitudeSTD_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencybodyGyroscopemagnitudeMeanFrequency_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencybodyGyroscopeJerkmagnitudeMean_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencybodyGyroscopeJerkmagnitudeSTD_Mean
        16
        Range -1 to 1, floating point number
        
* FrequencybodyGyroscopeJerkmagnitudeMeanFrequency_Mean
        16
        Range -1 to 1, floating point number
        
* AngleTimeBodyAccelerationMeanGravity_Mean
        16
        Range -1 to 1, floating point number
        
* AngleTimeBodyAccelerationJerkMeanGravityMean_Mean
        16
        Range -1 to 1, floating point number
        
* AngleTimeBodyGyroscopeMeanGravityMean_Mean
        16
        Range -1 to 1, floating point number
        
* AngleTimeBodyGyroscopeJerkMeanGravityMean_Mean
        16
        Range -1 to 1, floating point number
        
* AngleXGravityMean_Mean
        16
        Range -1 to 1, floating point number
        
* AngleYGravityMean_Mean
        16
        Range -1 to 1, floating point number
        
* AngleZGravityMean_Mean
        16
        Range -1 to 1, floating point number
        

-- End of variables --
