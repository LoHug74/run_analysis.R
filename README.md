# run_analysis.R
### Coursera R Getting and Cleansing Assigment Repo
### Getting and Cleaning Data Week 4 Assignment

## Assignment review criteria
* The submitted data set is tidy.
* The Github repo contains the required scripts.
* GitHub contains a code book that modifies and updates the available codebooks with the data to indicate all the variables and summaries         
  calculated, along with units, and any other relevant information.
* The README that explains the analysis files is clear and understandable.
* The work submitted for this project is the work of the student who submitted it.

Please find below the cleansing steps 
## Preparation: Data Download
* set working directory to shorten future paths
* download file, test if destination exists or not before
* unzip file and save it in the same folder
* get a list of all the zipped files

## Question 1
### Merge the training and the test sets to create one data set.
#### Extract meta data
* Feature names
* Activity names
#### Extract data
* read test data
* train data
#### Union Test & Train data sets
#### Name fields
#### Combine data sets columns

## Question 2: 
### Extracts only the measurements on the mean and standard deviation for each measurement.
* get list of relevant fields, ie, the ones containing mean () or std() 
* keep only relevant fields

## Question 3 
### Use descriptive activity names to name the activities in the data set
* join activity code to activity description
* check data set 

## Question 4 
### Appropriately labels the data set with descriptive variable names.
#### eg: make filed name such as "fBodyBodyGyroJerkMag" more readable
* 'f' becomes' frequency
* 'BodyBody' becomes body
* 'Gyro' becomes gyroscope
* 'Mag' becomes magnitude
* 't' becomes time
* 'Acc' becomes accelerometer
* '_' between description words to make it more readable

* check name change

## question 5 
### From the data set in step 4, 
### creates a second, independent tidy data set with the average of each variable for each activity and each subject.
* find replace NA by 0 in the dataset
* aggregate data set and compute mean
* write output table
