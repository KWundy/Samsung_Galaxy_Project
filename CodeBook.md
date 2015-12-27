Code book
=================
The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

tBodyAcc-XYZ
tGravityAcc-XYZ
tBodyAccJerk-XYZ
tBodyGyro-XYZ
tBodyGyroJerk-XYZ
tBodyAccMag
tGravityAccMag
tBodyAccJerkMag
tBodyGyroMag
tBodyGyroJerkMag
fBodyAcc-XYZ
fBodyAccJerk-XYZ
fBodyGyro-XYZ
fBodyAccMag
fBodyAccJerkMag
fBodyGyroMag
fBodyGyroJerkMag


The set of variables that were estimated from these signals are: 

_The first 53 entries_ of the averages tidy data are the correspond to the mean labels:
[1] "X.tBodyAcc.mean...X."                    "X.tBodyAcc.mean...Y."                   
 [3] "X.tBodyAcc.mean...Z."                    "X.tGravityAcc.mean...X."                
 [5] "X.tGravityAcc.mean...Y."                 "X.tGravityAcc.mean...Z."                
 [7] "X.tBodyAccJerk.mean...X."                "X.tBodyAccJerk.mean...Y."               
 [9] "X.tBodyAccJerk.mean...Z."                "X.tBodyGyro.mean...X."                  
[11] "X.tBodyGyro.mean...Y."                   "X.tBodyGyro.mean...Z."                  
[13] "X.tBodyGyroJerk.mean...X."               "X.tBodyGyroJerk.mean...Y."              
[15] "X.tBodyGyroJerk.mean...Z."               "X.tBodyAccMag.mean..."                  
[17] "X.tGravityAccMag.mean..."                "X.tBodyAccJerkMag.mean..."              
[19] "X.tBodyGyroMag.mean..."                  "X.tBodyGyroJerkMag.mean..."             
[21] "X.fBodyAcc.mean...X."                    "X.fBodyAcc.mean...Y."                   
[23] "X.fBodyAcc.mean...Z."                    "X.fBodyAcc.meanFreq...X."               
[25] "X.fBodyAcc.meanFreq...Y."                "X.fBodyAcc.meanFreq...Z."               
[27] "X.fBodyAccJerk.mean...X."                "X.fBodyAccJerk.mean...Y."               
[29] "X.fBodyAccJerk.mean...Z."                "X.fBodyAccJerk.meanFreq...X."           
[31] "X.fBodyAccJerk.meanFreq...Y."            "X.fBodyAccJerk.meanFreq...Z."           
[33] "X.fBodyGyro.mean...X."                   "X.fBodyGyro.mean...Y."                  
[35] "X.fBodyGyro.mean...Z."                   "X.fBodyGyro.meanFreq...X."              
[37] "X.fBodyGyro.meanFreq...Y."               "X.fBodyGyro.meanFreq...Z."              
[39] "X.fBodyAccMag.mean..."                   "X.fBodyAccMag.meanFreq..."              
[41] "X.fBodyBodyAccJerkMag.mean..."           "X.fBodyBodyAccJerkMag.meanFreq..."      
[43] "X.fBodyBodyGyroMag.mean..."              "X.fBodyBodyGyroMag.meanFreq..."         
[45] "X.fBodyBodyGyroJerkMag.mean..."          "X.fBodyBodyGyroJerkMag.meanFreq..."     
[47] "X.angle.tBodyAccMean.gravity.."          "X.angle.tBodyAccJerkMean..gravityMean.."
[49] "X.angle.tBodyGyroMean.gravityMean.."     "X.angle.tBodyGyroJerkMean.gravityMean.."
[51] "X.angle.X.gravityMean.."                 "X.angle.Y.gravityMean.."                
[53] "X.angle.Z.gravityMean.."                
std(): Standard deviation

_The last 33 entries_ of the average tidy data correspond to the standard deviation labels:

 [1] "X.tBodyAcc.std...X."           "X.tBodyAcc.std...Y."           "X.tBodyAcc.std...Z."          
 [4] "X.tGravityAcc.std...X."        "X.tGravityAcc.std...Y."        "X.tGravityAcc.std...Z."       
 [7] "X.tBodyAccJerk.std...X."       "X.tBodyAccJerk.std...Y."       "X.tBodyAccJerk.std...Z."      
[10] "X.tBodyGyro.std...X."          "X.tBodyGyro.std...Y."          "X.tBodyGyro.std...Z."         
[13] "X.tBodyGyroJerk.std...X."      "X.tBodyGyroJerk.std...Y."      "X.tBodyGyroJerk.std...Z."     
[16] "X.tBodyAccMag.std..."          "X.tGravityAccMag.std..."       "X.tBodyAccJerkMag.std..."     
[19] "X.tBodyGyroMag.std..."         "X.tBodyGyroJerkMag.std..."     "X.fBodyAcc.std...X."          
[22] "X.fBodyAcc.std...Y."           "X.fBodyAcc.std...Z."           "X.fBodyAccJerk.std...X."      
[25] "X.fBodyAccJerk.std...Y."       "X.fBodyAccJerk.std...Z."       "X.fBodyGyro.std...X."         
[28] "X.fBodyGyro.std...Y."          "X.fBodyGyro.std...Z."          "X.fBodyAccMag.std..."         
[31] "X.fBodyBodyAccJerkMag.std..."  "X.fBodyBodyGyroMag.std..."     "X.fBodyBodyGyroJerkMag.std..."
