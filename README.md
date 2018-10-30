# Human Activity Recognition using smart-phones

## Problem-Statement
Human Activity Recognition (HAR) using smartphones dataset and an LSTM RNN. Classifying the type of movement amongst six categories(multi-class classification).

**Six-Categories:**
 
* WALKING,
* WALKING_UPSTAIRS,
* WALKING_DOWNSTAIRS,
* SITTING,
* STANDING,
* LAYING.


### About Data:
This dataset is collected from 30 persons, performing different activities with a smartphone to their waists. The data is recorded with the help of sensors (accelerometer and Gyroscope) in that smartphone.

* Accelerometer readings are divided into total acceleration and body acceleration readings, which has x,y and z components each.
* Gyroscope readings are the measure of angular velocities which has x,y and z components.
* Pre-processing accelerometer and gyroscope readings using noise filters.
* Splitting data into fixed windows of 2.56 seconds (128 data points) with 50% overlap.Splitting of accelerometer data into gravitational (total) and body motion components


## Train and Test Split

* The dataset was split into train (70%) and test (30%) sets based on data for subjects, e.g. 21 Persons data for train and 9 persons data for test.
* Each data-point corresponds to one of the six-activities
* 7352 train and 2947 test samples


### Note
* There are three main signal types in the raw data: total acceleration, body acceleration, and body gyroscope. Each has 3 axises of data. This means that there are a total of nine variables for each time step.

* one row of data has (128 * 9), or 1,152 elements.

Data
All the data is present in 'UCI_HAR_dataset/' 
Feature names are present in 'UCI_HAR_dataset/features.txt'
Train Data
'UCI_HAR_dataset/train/X_train.txt'
'UCI_HAR_dataset/train/subject_train.txt'
'UCI_HAR_dataset/train/y_train.txt'
Test Data
'UCI_HAR_dataset/test/X_test.txt'
'UCI_HAR_dataset/test/subject_test.txt'
'UCI_HAR_dataset/test/y_test.txt'


###  class_labels
+ In the dataset, class_labels are represented as numbers from 1 to 6 as their identifiers.

	- WALKING as __1__
	- WALKING_UPSTAIRS as __2__
	- WALKING_DOWNSTAIRS as __3__
	- SITTING as __4__
	- STANDING as __5__
	- LAYING as __6__
