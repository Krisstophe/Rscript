How the script works
===========
This is a guide about how to use "run_analysis.R" script to get tidy data.

1. Click the download file "getdata-projectfiles-UCI HAR Dataset" to expand it, and you'll have a folder "UCI HAR Dataset" with another two folders and four text files in it.
2. Open Rstudio.
3. File -> Open File, load the script "run_analysis.R".
4. Use setwd command to set "UCI HAR Dataset" as your working directory in the console window.
5. Run script.
6. After R studio's work, you'll get a tidy data named "tidydata.txt" in your working directory.

GOOD LUCK!
===========

Explanation of the script
===========

1. Use <cbind> to merge three test files and three train files into two files "test" and "train".
2. Use <rbind> to merge "test" and "train" into "data".
3. Read "features.txt" to get variable names.
4. Use <grepl> to select "std" and "mean" columns.
5. Use <gsub> six times to replace activitylabels by descriptive language.
6. Use <grep> and <colnames> to replace variable column names by descriptive language.
7. Use <melt> and <dcast> of reshape2 to get mean values of defined group.
