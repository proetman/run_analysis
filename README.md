---
title: "README.md"
author: "Paul Roetman"
date: "15 June 2017"
output: html_document
---


## Readme.md


### Run Analyse

The program run_analyse.R can be run in any R environment. Before running, the global variable need to be configured at the beginning of the program. This variable defines where the data will be read from, and where the results will be written.

```{r}
dir_proj_data <- 'C:/temp/UCI HAR Dataset'
```
To run the program:

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
