# Getting and Cleaning Data Course Project
Several Steps were taken in order to transform the initial data set. The test & train sets were merged, & the subject identifiers/activity labels were pulled in to create a single data set. The activity identifiers were transformed from identifiers to readable names.
Of all the variables present, only the mean and standard deviation were kept.
These variables were further summarised by taking the mean for each subject/activity pair.

The final data set is found in the 'tidy_data.txt' file, which can be read using `read.table("tidy_data.txt", header = T)`.

A detailed discription can be found in `Code_Book.txt`. The naming convention is:

  mean{time/freq}{measument}{mean/std}{X/Y/Z}

`Time/Freq` indicates whether a measurement comes from the time or the frequency domain
`Measuement` indicates the original measurement featur
`Mean/Std` indicates whether a measuement was a mean or a standard deviation variable
`X/Y/Z` indicates the axis from which the measurement was taken (or nothing, for magnitude measurments)
