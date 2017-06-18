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

While the original data contained many more variables, the only data retained for this result set were the variables pertaining to either Mean (Mean) or Standard deviation (STD). 

The data from train and the data from test were loaded and concatenated together, then the mean data was extracted per subject per activity. This new data set is written to the file "results.txt".

* Subject
* Activity
* TimeBodyAccelerationMeanX_Mean
* TimeBodyAccelerationMeanY_Mean
* TimeBodyAccelerationMeanZ_Mean
* TimeBodyAccelerationSTDX_Mean
* TimeBodyAccelerationSTDY_Mean
* TimeBodyAccelerationSTDZ_Mean
* TimeGravityAccelerationMeanX_Mean
* TimeGravityAccelerationMeanY_Mean
* TimeGravityAccelerationMeanZ_Mean
* TimeGravityAccelerationSTDX_Mean
* TimeGravityAccelerationSTDY_Mean
* TimeGravityAccelerationSTDZ_Mean
* TimeBodyAccelerationJerkMeanX_Mean
* TimeBodyAccelerationJerkMeanY_Mean
* TimeBodyAccelerationJerkMeanZ_Mean
* TimeBodyAccelerationJerkSTDX_Mean
* TimeBodyAccelerationJerkSTDY_Mean
* TimeBodyAccelerationJerkSTDZ_Mean
* TimeBodyGyroscopeMeanX_Mean
* TimeBodyGyroscopeMeanY_Mean
* TimeBodyGyroscopeMeanZ_Mean
* TimeBodyGyroscopeSTDX_Mean
* TimeBodyGyroscopeSTDY_Mean
* TimeBodyGyroscopeSTDZ_Mean
* TimeBodyGyroscopeJerkMeanX_Mean
* TimeBodyGyroscopeJerkMeanY_Mean
* TimeBodyGyroscopeJerkMeanZ_Mean
* TimeBodyGyroscopeJerkSTDX_Mean
* TimeBodyGyroscopeJerkSTDY_Mean
* TimeBodyGyroscopeJerkSTDZ_Mean
* TimeBodyAccelerationmagnitudeMean_Mean
* TimeBodyAccelerationmagnitudeSTD_Mean
* TimeGravityAccelerationmagnitudeMean_Mean
* TimeGravityAccelerationmagnitudeSTD_Mean
* TimeBodyAccelerationJerkmagnitudeMean_Mean
* TimeBodyAccelerationJerkmagnitudeSTD_Mean
* TimeBodyGyroscopemagnitudeMean_Mean
* TimeBodyGyroscopemagnitudeSTD_Mean
* TimeBodyGyroscopeJerkmagnitudeMean_Mean
* TimeBodyGyroscopeJerkmagnitudeSTD_Mean
* FrequencyBodyAccelerationMeanX_Mean
* FrequencyBodyAccelerationMeanY_Mean
* FrequencyBodyAccelerationMeanZ_Mean
* FrequencyBodyAccelerationSTDX_Mean
* FrequencyBodyAccelerationSTDY_Mean
* FrequencyBodyAccelerationSTDZ_Mean
* FrequencyBodyAccelerationMeanFrequencyX_Mean
* FrequencyBodyAccelerationMeanFrequencyY_Mean
* FrequencyBodyAccelerationMeanFrequencyZ_Mean
* FrequencyBodyAccelerationJerkMeanX_Mean
* FrequencyBodyAccelerationJerkMeanY_Mean
* FrequencyBodyAccelerationJerkMeanZ_Mean
* FrequencyBodyAccelerationJerkSTDX_Mean
* FrequencyBodyAccelerationJerkSTDY_Mean
* FrequencyBodyAccelerationJerkSTDZ_Mean
* FrequencyBodyAccelerationJerkMeanFrequencyX_Mean
* FrequencyBodyAccelerationJerkMeanFrequencyY_Mean
* FrequencyBodyAccelerationJerkMeanFrequencyZ_Mean
* FrequencyBodyGyroscopeMeanX_Mean
* FrequencyBodyGyroscopeMeanY_Mean
* FrequencyBodyGyroscopeMeanZ_Mean
* FrequencyBodyGyroscopeSTDX_Mean
* FrequencyBodyGyroscopeSTDY_Mean
* FrequencyBodyGyroscopeSTDZ_Mean
* FrequencyBodyGyroscopeMeanFrequencyX_Mean
* FrequencyBodyGyroscopeMeanFrequencyY_Mean
* FrequencyBodyGyroscopeMeanFrequencyZ_Mean
* FrequencyBodyAccelerationmagnitudeMean_Mean
* FrequencyBodyAccelerationmagnitudeSTD_Mean
* FrequencyBodyAccelerationmagnitudeMeanFrequency_Mean
* FrequencybodyAccelerationJerkmagnitudeMean_Mean
* FrequencybodyAccelerationJerkmagnitudeSTD_Mean
* FrequencybodyAccelerationJerkmagnitudeMeanFrequency_Mean
* FrequencybodyGyroscopemagnitudeMean_Mean
* FrequencybodyGyroscopemagnitudeSTD_Mean
* FrequencybodyGyroscopemagnitudeMeanFrequency_Mean
* FrequencybodyGyroscopeJerkmagnitudeMean_Mean
* FrequencybodyGyroscopeJerkmagnitudeSTD_Mean
* FrequencybodyGyroscopeJerkmagnitudeMeanFrequency_Mean
* AngleTimeBodyAccelerationMeanGravity_Mean
* AngleTimeBodyAccelerationJerkMeanGravityMean_Mean
* AngleTimeBodyGyroscopeMeanGravityMean_Mean
* AngleTimeBodyGyroscopeJerkMeanGravityMean_Mean
* AngleXGravityMean_Mean
* AngleYGravityMean_Mean
* AngleZGravityMean_Mean

-- End of variables --
