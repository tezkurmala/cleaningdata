DATA DICTIONARY - Human Activity Recognition Using Smartphones
==============================================================
**Subject** 2 
 Record Type
 1..30 An entity who carried out the experiment
**Activity** 18 
 Activity the subject was performing when the observation was taken.
 Following are valid values.
 WALKING
 WALKING_UPSTAIRS
 WALKING_DOWNSTAIRS
 SITTING
 STANDING
 LAYING
**timeBodyAccelerometerMeanOfX** 13
 Average of body acceleration signals captured over an accelerometer on axial X.
 Time domain signals were captured over an accelerometer at a constant rate of 50 Hz and then filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. The acceleration signals obtained from accelerometer was then separated into body and gravity acceleration signals using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 
 -1..1
**timeBodyAccelerometerMeanOfY** 13
 Average of body acceleration signals captured over an accelerometer on axial Y.
 -1..1
**timeBodyAccelerometerMeanOfZ** 13
 Average of body acceleration signals captured over an accelerometer on axial Z.
 -1..1
**timeBodyAccelerometerStandardDeviationOfX** 13
 Standard Deviation of body acceleration signals captured over an accelerometer on axial X.
 -1..1
**timeBodyAccelerometerStandardDeviationOfY** 13
 Standard Deviation of body acceleration signals captured over an accelerometer on axial Y.
 -1..1
**timeBodyAccelerometerStandardDeviationOfZ** 13
 Standard Deviation of body acceleration signals captured over an accelerometer on axial Z.
 -1..1
**timeGravityAccelerometerMeanOfX** 13
  Average of gravity acceleration signals captured over an accelerometer on axial X.
 -1..1
**timeGravityAccelerometerMeanOfY** 13
  Average of gravity acceleration signals captured over an accelerometer on axial Y.
 -1..1
**timeGravityAccelerometerMeanOfZ** 13
  Average of gravity acceleration signals captured over an accelerometer on axial Z.
 -1..1
**timeGravityAccelerometerStandardDeviationOfX** 13
  Standard Deviation of gravity acceleration signals captured over an accelerometer on axial X.
 -1..1
**timeGravityAccelerometerStandardDeviationOfY** 13
  Standard Deviation of gravity acceleration signals captured over an accelerometer on axial Y.
 -1..1
**timeGravityAccelerometerStandardDeviationOfZ** 13
  Standard Deviation of gravity acceleration signals captured over an accelerometer on axial Z.
 -1..1
**timeBodyAccelerometerJerkMeanOfX** 13
  Average of body linear acceleration and angular velocity using accelerometer derived in time to obtain Jerk signals over axial X. 
 -1..1
**timeBodyAccelerometerJerkMeanOfY** 13
  Average of body linear acceleration and angular velocity using accelerometer derived in time to obtain Jerk signals over axial Y.
 -1..1
**timeBodyAccelerometerJerkMeanOfZ** 13
  Average of body linear acceleration and angular velocity using accelerometer derived in time to obtain Jerk signals over axial Z.
 -1..1
**timeBodyAccelerometerJerkStandardDeviationOfX** 13
  Standard Deviation of body linear acceleration and angular velocity using accelerometer derived in time to obtain Jerk signals over axial X.
 -1..1
**timeBodyAccelerometerJerkStandardDeviationOfY** 13
  Standard Deviation of body linear acceleration and angular velocity using accelerometer derived in time to obtain Jerk signals over axial Y.
 -1..1
**timeBodyAccelerometerJerkStandardDeviationOfZ** 13
  Standard Deviation of body linear acceleration and angular velocity using accelerometer derived in time to obtain Jerk signals over axial Z.
 -1..1
**timeBodyGyroscopeMeanOfX** 13
  Average of body acceleration signals captured over an Gyroscope on axial X.
 -1..1
**timeBodyGyroscopeMeanOfY** 13
  Average of body acceleration signals captured over an Gyroscope on axial Y.
 -1..1
**timeBodyGyroscopeMeanOfZ** 13
  Average of body acceleration signals captured over an Gyroscope on axial Z.
 -1..1
**timeBodyGyroscopeStandardDeviationOfX** 13
  Standard Deviation of body acceleration signals captured over an Gyroscope on axial X.
 -1..1
**timeBodyGyroscopeStandardDeviationOfY** 13
  Standard Deviation of body acceleration signals captured over an Gyroscope on axial Y.
 -1..1
**timeBodyGyroscopeStandardDeviationOfZ** 13
  Standard Deviation of body acceleration signals captured over an Gyroscope on axial Z.
 -1..1
**timeBodyGyroscopeJerkMeanOfX** 13
  Average of body linear acceleration and angular velocity using Gyroscope derived in time to obtain Jerk signals over axial X.
 -1..1
**timeBodyGyroscopeJerkMeanOfY** 13
  Average of body linear acceleration and angular velocity using Gyroscope derived in time to obtain Jerk signals over axial Y.
 -1..1
**timeBodyGyroscopeJerkMeanOfZ** 13
  Average of body linear acceleration and angular velocity using Gyroscope derived in time to obtain Jerk signals over axial Z.
 -1..1
**timeBodyGyroscopeJerkStandardDeviationOfX** 13
  Standard Deviation of body linear acceleration and angular velocity using Gyroscope derived in time to obtain Jerk signals over axial X.
 -1..1
**timeBodyGyroscopeJerkStandardDeviationOfY** 13
  Standard Deviation of body linear acceleration and angular velocity using Gyroscope derived in time to obtain Jerk signals over axial Y.
 -1..1
**timeBodyGyroscopeJerkStandardDeviationOfZ** 13
  Standard Deviation of body linear acceleration and angular velocity using Gyroscope derived in time to obtain Jerk signals over axial Z.
 -1..1
**timeBodyAccelerometerMagnitudeMean** 13
 Average of the magnitude of X,Y,Z dimensional body acceleration signals captured over Accelerometer calculated using the Euclidean norm.
 -1..1
**timeBodyAccelerometerMagnitudeStandardDeviation** 13
 Standard Deviation of the magnitude of these X,Y,Z dimensional body acceleration signals captured over Accelerometer calculated using the Euclidean norm.
 -1..1
**timeGravityAccelerometerMagnitudeMean** 13
 Average of the magnitude of X,Y,Z dimensional gravity acceleration signals captured over Accelerometer calculated using the Euclidean norm.
 -1..1
**timeGravityAccelerometerMagnitudeStandardDeviation** 13
 Standard Deviation of the magnitude of these X,Y,Z dimensional gravity acceleration signals captured over Accelerometer calculated using the Euclidean norm.
 -1..1
**timeBodyAccelerometerJerkMagnitudeMean** 13
  Average of the magnitude of X,Y,Z dimensional body linear acceleration and angular velocity using Accelerometer derived in time to obtain Jerk signals.
 -1..1
**timeBodyAccelerometerJerkMagnitudeStandardDeviation** 13
  Standard Deviation of the magnitude of X,Y,Z dimensional body linear acceleration and angular velocity using Accelerometer derived in time to obtain Jerk signals.
 -1..1
**timeBodyGyroscopeMagnitudeMean** 13
 Average of the magnitude of X,Y,Z dimensional body acceleration signals captured over Gyroscope calculated using the Euclidean norm.
 -1..1
**timeBodyGyroscopeMagnitudeStandardDeviation** 13
 Standard Deviation of the magnitude of X,Y,Z dimensional body acceleration signals captured over Gyroscope calculated using the Euclidean norm.
 -1..1
**timeBodyGyroscopeJerkMagnitudeMean** 13
  Average of the magnitude of X,Y,Z dimensional body linear acceleration and angular velocity using Gyroscope derived in time to obtain Jerk signals.
 -1..1
**timeBodyGyroscopeJerkMagnitudeStandardDeviation** 13
  Standard Deviation of the magnitude of X,Y,Z dimensional body linear acceleration and angular velocity using Gyroscope derived in time to obtain Jerk signals.
 -1..1
**frequencyBodyAccelerometerMeanOfX** 13
 Average of Fast Fourier Transform (applied to body acceleration signals) captured over an accelerometer on axial X.
 -1..1
frequencyBodyAccelerometerMeanOfY** 13
 Average of Fast Fourier Transform (applied to body acceleration signals) captured over an accelerometer on axial Y.
 -1..1
**frequencyBodyAccelerometerMeanOfZ** 13
 Average of Fast Fourier Transform (applied to body acceleration signals) captured over an accelerometer on axial Z.
 -1..1
**frequencyBodyAccelerometerStandardDeviationOfX** 13
 Standard Deviation of Fast Fourier Transform (applied to body acceleration signals) captured over an accelerometer on axial X.
 -1..1
**frequencyBodyAccelerometerStandardDeviationOfY** 13
 Standard Deviation of Fast Fourier Transform (applied to body acceleration signals) captured over an accelerometer on axial Y.
 -1..1
**frequencyBodyAccelerometerStandardDeviationOfZ** 13
 Standard Deviation of Fast Fourier Transform (applied to body acceleration signals) captured over an accelerometer on axial Z.
 -1..1
**frequencyBodyAccelerometerJerkMeanOfX** 13
  Average of Fast Fourier Transform (applied to body linear acceleration and angular velocity) using accelerometer derived in time to obtain Jerk signals over axial X.
 -1..1
**frequencyBodyAccelerometerJerkMeanOfY** 13
  Average of Fast Fourier Transform (applied to body linear acceleration and angular velocity) using accelerometer derived in time to obtain Jerk signals over axial Y.
 -1..1
**frequencyBodyAccelerometerJerkMeanOfZ** 13
  Average of Fast Fourier Transform (applied to body linear acceleration and angular velocity) using accelerometer derived in time to obtain Jerk signals over axial Z.
 -1..1
**frequencyBodyAccelerometerJerkStandardDeviationOfX** 13
  Standard Deviation of Fast Fourier Transform (applied to body linear acceleration and angular velocity) using accelerometer derived in time to obtain Jerk signals over axial X.
 -1..1
**frequencyBodyAccelerometerJerkStandardDeviationOfY** 13
  Standard Deviation of Fast Fourier Transform (applied to body linear acceleration and angular velocity) using accelerometer derived in time to obtain Jerk signals over axial Y.
 -1..1
**frequencyBodyAccelerometerJerkStandardDeviationOfZ** 13
  Standard Deviation of Fast Fourier Transform (applied to body linear acceleration and angular velocity) using accelerometer derived in time to obtain Jerk signals over axial Z.
 -1..1
**frequencyBodyGyroscopeMeanOfX** 13
 Average of Fast Fourier Transform (applied to body acceleration signals) captured over an Gyroscope on axial X.
 -1..1
**frequencyBodyGyroscopeMeanOfY** 13
 Average of Fast Fourier Transform (applied to body acceleration signals) captured over an Gyroscope on axial Y.
 -1..1
**frequencyBodyGyroscopeMeanOfZ** 13
 Average of Fast Fourier Transform (applied to body acceleration signals) captured over an Gyroscope on axial Z.
 -1..1
**frequencyBodyGyroscopeStandardDeviationOfX** 13
 Standard Deviation of Fast Fourier Transform (applied to body acceleration signals) captured over an Gyroscope on axial X.
 -1..1
**frequencyBodyGyroscopeStandardDeviationOfY** 13
 Standard Deviation of Fast Fourier Transform (applied to body acceleration signals) captured over an Gyroscope on axial Y.
 -1..1
**frequencyBodyGyroscopeStandardDeviationOfZ** 13
 Standard Deviation of Fast Fourier Transform (applied to body acceleration signals) captured over an Gyroscope on axial Z.
 -1..1
**frequencyBodyAccelerometerMagnitudeMean** 13
 Average of Fast Fourier Transform applied to the magnitude of X,Y,Z dimensional body acceleration signals captured over Accelerometer calculated using the Euclidean norm.
 -1..1
**frequencyBodyAccelerometerMagnitudeStandardDeviation** 13
 Standard Deviation of Fast Fourier Transform applied to the magnitude of X,Y,Z dimensional body acceleration signals captured over Accelerometer calculated using the Euclidean norm.
 -1..1
**frequencyBodyBodyAccelerometerJerkMagnitudeMean** 13
 Average of Fast Fourier Transform applied to the magnitude of X,Y,Z dimensional body linear acceleration and angular velocity using Accelerometer derived in time to obtain Jerk signals.
 -1..1
**frequencyBodyBodyAccelerometerJerkMagnitudeStandardDeviation** 13
 Standard Deviation of Fast Fourier Transform applied to the magnitude of X,Y,Z dimensional body linear acceleration and angular velocity using Accelerometer derived in time to obtain Jerk signals.
 -1..1
**frequencyBodyBodyGyroscopeMagnitudeMean** 13
 Average of Fast Fourier Transform applied to the magnitude of X,Y,Z dimensional body acceleration signals captured over Gyroscope calculated using the Euclidean norm.
 -1..1
**frequencyBodyBodyGyroscopeMagnitudeStandardDeviation** 13
 Standard Deviation of Fast Fourier Transform applied to the magnitude of X,Y,Z dimensional body acceleration signals captured over Gyroscope calculated using the Euclidean norm.
 -1..1
**frequencyBodyBodyGyroscopeJerkMagnitudeMean** 13
 Average of Fast Fourier Transform applied to the magnitude of X,Y,Z dimensional body linear acceleration and angular velocity using Gyroscope derived in time to obtain Jerk signals.
 -1..1
**frequencyBodyBodyGyroscopeJerkMagnitudeStandardDeviation** 13
 Standard Deviation of Fast Fourier Transform applied to the magnitude of X,Y,Z dimensional body linear acceleration and angular velocity using Gyroscope derived in time to obtain Jerk signals.
 -1..1
 
*Note: Values for each variable are averages grouped by Subject and Activity.*