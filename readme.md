Getting and Cleaning Data Course Project
========================================

The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. You will be graded by your peers on a series of yes/no questions related to the project. You will be required to submit: 1) a tidy data set as described below, 2) a link to a Github repository with your script for performing the analysis, and 3) a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data called CodeBook.md. You should also include a README.md in the repo with your scripts. This repo explains how all of the scripts work and how they are connected.

One of the most exciting areas in all of data science right now is wearable computing - see for example this article ( http://www.insideactivitytracking.com/data-science-activity-tracking-and-the-battle-for-the-worlds-top-sports-brand/ ). Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained: 

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

Here are the data for the project: 

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

You should create one R script called run_analysis.R that does the following. 

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names.
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

## Solution proposed

In this repository you'll find my solution code, with the following files:
* run_analysis.R

This solution uses the following packages:
* plyr
* data.table
* reshape2

Steps to run this solution:
1. Clone this project on your HD, and set as working directory.
2. Download and Unzip dataset on your working directory.
3. Load file **`source("run_analysis.R")`**
4. Execute **`run.analysis()`**
5. New file "kkkkkk.txt" will be created on your working directory

* Unzip the file getdata-projectfiles-UCI HAR Dataset.zip in your working directory.
* Place the scripts *run_analysis.R*, *analysis_functions.R* and *constants.R* in your working directory.
* If necessary, modify the file *constants.R* indicating the name of the directory containing the data, if it has been modified, and / or the delimiting character for your filesystem.
* Load the source *run_analysis.R* at your session in R, with **`source("run_analysis.R")`**
* Finally, execute **`run.analysis()`** in R.
* Be sure to have installed the packages data.table, plyr and reshape2.

run.analysis() uses the constants defined in constants.R and the functions from analysis_functions.R, and generates a file called new_dataset.txt in your working directory.