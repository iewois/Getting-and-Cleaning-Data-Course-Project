# Code book for Getting and Cleaning Data Coursera Course Project

The data set that this code book pertains to is located in the tidy_data.txt file of this repository.
See the README.md file of this repository for background information on this data set.
The structure of the data set is described in the Data section, its variables are listed in the Variables section, and the transformations that were carried out to obtain the data set based on the source data are presented in the Transformations section.

# Data
The tidy_data.txt data file is a text file, containing space-separated values.
The first row contains the names of the variables, which are listed and described in the Variables section, and the following rows contain the values of these variables.

# Variables
Each row contains, for a given subject and activity, 79 averaged signal measurements.

# Identifiers
1. subject
Subject identifier, integer, ranges from 1 to 30.

2. activity
Activity identifier, string with 6 possible values:
1. WALKING: subject was walking
2. WALKING_UPSTAIRS: subject was walking upstairs
3. WALKING_DOWNSTAIRS: subject was walking downstairs
4. SITTING: subject was sitting
5. STANDING: subject was standing
6. LAYING: subject was laying

# Average of measurements
All measurements are floating-point values, normalised and bounded within [-1,1].

Prior to normalisation, acceleration measurements (variables containing Accelerometer) were made in g's (9.81 m.s⁻²) and gyroscope measurements (variables containing Gyroscope) were made in radians per second (rad.s⁻¹).

Magnitudes of three-dimensional signals (variables containing Magnitude) were calculated using the Euclidean norm.

The measurements are classified in two domains:
1. Time-domain signals (variables prefixed by timeDomain), resulting from the capture of accelerometer and gyroscope raw signals.
2. Frequency-domain signals (variables prefixed by frequencyDomain), resulting from the application of a Fast Fourier Transform (FFT) to some of the time-domain signals.

# Time-domain signals
1. Average time-domain body acceleration in the X, Y and Z directions:
a. timeDomainBodyAccelerometerMeanX
b. timeDomainBodyAccelerometerMeanY
c. timeDomainBodyAccelerometerMeanZ

2. Standard deviation of the time-domain body acceleration in the X, Y and Z directions:
a. timeDomainBodyAccelerometerStandardDeviationX
b. timeDomainBodyAccelerometerStandardDeviationY
c. timeDomainBodyAccelerometerStandardDeviationZ

3. Average time-domain gravity acceleration in the X, Y and Z directions:
a. timeDomainGravityAccelerometerMeanX
b. timeDomainGravityAccelerometerMeanY
c. timeDomainGravityAccelerometerMeanZ

4. Standard deviation of the time-domain gravity acceleration in the X, Y and Z directions
a. timeDomainGravityAccelerometerStandardDeviationX
b. timeDomainGravityAccelerometerStandardDeviationY
c. timeDomainGravityAccelerometerStandardDeviationZ

5. Average time-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
a. timeDomainBodyAccelerometerJerkMeanX
b. timeDomainBodyAccelerometerJerkMeanY
c. timeDomainBodyAccelerometerJerkMeanZ

6. Standard deviation of the time-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
a. timeDomainBodyAccelerometerJerkStandardDeviationX
b. timeDomainBodyAccelerometerJerkStandardDeviationY
c. timeDomainBodyAccelerometerJerkStandardDeviationZ

7. Average time-domain body angular velocity in the X, Y and Z directions:
a. timeDomainBodyGyroscopeMeanX
b. timeDomainBodyGyroscopeMeanY
c. timeDomainBodyGyroscopeMeanZ

8. Standard deviation of the time-domain body angular velocity in the X, Y and Z directions:
a. timeDomainBodyGyroscopeStandardDeviationX
b. timeDomainBodyGyroscopeStandardDeviationY
c. timeDomainBodyGyroscopeStandardDeviationZ

9. Average time-domain body angular velocity jerk (derivation of the angular velocity in time) in the X, Y and Z directions:
a. timeDomainBodyGyroscopeJerkMeanX
b. timeDomainBodyGyroscopeJerkMeanY
c. timeDomainBodyGyroscopeJerkMeanZ

10. Standard deviation of the time-domain body angular velocity jerk (derivation of the angular velocity in time) in the X, Y and Z directions:
a. timeDomainBodyGyroscopeJerkStandardDeviationX
b. timeDomainBodyGyroscopeJerkStandardDeviationY
c. timeDomainBodyGyroscopeJerkStandardDeviationZ

11. Average and standard deviation of the time-domain magnitude of body acceleration:
a. timeDomainBodyAccelerometerMagnitudeMean
b. timeDomainBodyAccelerometerMagnitudeStandardDeviation

12. Average and standard deviation of the time-domain magnitude of gravity acceleration:
a. timeDomainGravityAccelerometerMagnitudeMean
b. timeDomainGravityAccelerometerMagnitudeStandardDeviation

13. Average and standard deviation of the time-domain magnitude of body acceleration jerk (derivation of the acceleration in time):
a. timeDomainBodyAccelerometerJerkMagnitudeMean
b. timeDomainBodyAccelerometerJerkMagnitudeStandardDeviation

14. Average and standard deviation of the time-domain magnitude of body angular velocity:
a. timeDomainBodyGyroscopeMagnitudeMean
b. timeDomainBodyGyroscopeMagnitudeStandardDeviation

15. Average and standard deviation of the time-domain magnitude of body angular velocity jerk (derivation of the angular velocity in time):
a. timeDomainBodyGyroscopeJerkMagnitudeMean
b. timeDomainBodyGyroscopeJerkMagnitudeStandardDeviation

# Frequency-domain signals
1. Average frequency-domain body acceleration in the X, Y and Z directions:
a. frequencyDomainBodyAccelerometerMeanX
b. frequencyDomainBodyAccelerometerMeanY
c. frequencyDomainBodyAccelerometerMeanZ

2. Standard deviation of the frequency-domain body acceleration in the X, Y and Z directions:
a. frequencyDomainBodyAccelerometerStandardDeviationX
b. frequencyDomainBodyAccelerometerStandardDeviationY
c. frequencyDomainBodyAccelerometerStandardDeviationZ

3. Weighted average of the frequency components of the frequency-domain body acceleration in the X, Y and Z directions:
a. frequencyDomainBodyAccelerometerMeanFrequencyX
b. frequencyDomainBodyAccelerometerMeanFrequencyY
c. frequencyDomainBodyAccelerometerMeanFrequencyZ

4. Average frequency-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
a. frequencyDomainBodyAccelerometerJerkMeanX
b. frequencyDomainBodyAccelerometerJerkMeanY
c. frequencyDomainBodyAccelerometerJerkMeanZ

5. Standard deviation of the frequency-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
a. frequencyDomainBodyAccelerometerJerkStandardDeviationX
b. frequencyDomainBodyAccelerometerJerkStandardDeviationY
c. frequencyDomainBodyAccelerometerJerkStandardDeviationZ

6. Weighted average of the frequency components of the frequency-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
a. frequencyDomainBodyAccelerometerJerkMeanFrequencyX
b. frequencyDomainBodyAccelerometerJerkMeanFrequencyY
c. frequencyDomainBodyAccelerometerJerkMeanFrequencyZ

7. Average frequency-domain body angular velocity in the X, Y and Z directions:
a. frequencyDomainBodyGyroscopeMeanX
b. frequencyDomainBodyGyroscopeMeanY
c. frequencyDomainBodyGyroscopeMeanZ

8. Standard deviation of the frequency-domain body angular velocity in the X, Y and Z directions:
a. frequencyDomainBodyGyroscopeStandardDeviationX
b. frequencyDomainBodyGyroscopeStandardDeviationY
c. frequencyDomainBodyGyroscopeStandardDeviationZ

9. Weighted average of the frequency components of the frequency-domain body angular velocity in the X, Y and Z directions:
a. frequencyDomainBodyGyroscopeMeanFrequencyX
b. frequencyDomainBodyGyroscopeMeanFrequencyY
c. frequencyDomainBodyGyroscopeMeanFrequencyZ

10. Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body acceleration:
a. frequencyDomainBodyAccelerometerMagnitudeMean
b. frequencyDomainBodyAccelerometerMagnitudeStandardDeviation
c. frequencyDomainBodyAccelerometerMagnitudeMeanFrequency

11. Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body acceleration jerk (derivation of the acceleration in time):
a. frequencyDomainBodyAccelerometerJerkMagnitudeMean
b. frequencyDomainBodyAccelerometerJerkMagnitudeStandardDeviation
c. frequencyDomainBodyAccelerometerJerkMagnitudeMeanFrequency

12. Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body angular velocity:
a. frequencyDomainBodyGyroscopeMagnitudeMean
b. frequencyDomainBodyGyroscopeMagnitudeStandardDeviation
c. frequencyDomainBodyGyroscopeMagnitudeMeanFrequency

13. Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body angular velocity jerk (derivation of the angular velocity in time):
a. frequencyDomainBodyGyroscopeJerkMagnitudeMean
b. frequencyDomainBodyGyroscopeJerkMagnitudeStandardDeviation
c. frequencyDomainBodyGyroscopeJerkMagnitudeMeanFrequency

# Transformations
The zip file containing the source data is located at https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.

The following transformations were applied to the source data:

1. The training and test sets were merged to create one data set.
2. The measurements on the mean and standard deviation (i.e. signals containing the strings mean and std) were extracted for each measurement, and the others were discarded.
3. The activity identifiers (originally coded as integers between 1 and 6) were replaced with descriptive activity names (see Identifiers section).
4. The variable names were replaced with descriptive variable names (e.g. tBodyAcc-mean()-X was expanded to timeDomainBodyAccelerometerMeanX), using the following set of rules:
a. Special characters (i.e. (, ), and -) were removed
b. The initial f and t were expanded to frequencyDomain and timeDomain respectively.
c. Acc, Gyro, Mag, Freq, mean, and std were replaced with Accelerometer, Gyroscope, Magnitude, Frequency, Mean, and StandardDeviation respectively.
d. Replaced (supposedly incorrect as per source's features_info.txt file) BodyBody with Body.
5. From the data set in step 4, the final data set was created with the average of each variable for each activity and each subject.

The collection of the source data and the transformations listed above were implemented by the run_analysis.R R script (see README.md file for usage instructions).
