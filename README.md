---
title: "README.md"
author: "Paul Roetman"
date: "15 June 2017"
output: html_document
---


## Readme.md


### Run Analyse

The program run_analyse.R can be run in any R environment. The program makes the assumption that the code is in the directory where the data has been extracted. For example, if the data is in this directory:
    "c:\temp\UCI HAR Dataset"
then copy the run_analysis.R program to this directory as well.

To run the program, load the R environment then:

```{r}
source('run_analysis.R')
run_analysis()
```

Once the program has been completed, the results.txt file can be viewed with an editor, or loaded into a data set in R with this command:

```{r}
data <- read.table('results.txt', sep=" ", header=TRUE)
summary(data)
```

### Other relevent Files
### 
#### README.md
This file, containing information on how to run the program, and view the data.

#### codeBook.md

Document the variables in the results.txt file, and defines how the data is created.
