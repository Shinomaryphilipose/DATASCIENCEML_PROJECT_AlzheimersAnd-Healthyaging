The dataset I took for this project is Alzheimer_s_Disease_and_Healthy_Aging_Data.csv from the healthdata.gov site.
This data collected by The_Behavioral_Risk_Factor_Surveillance_System (BRFSS)contains results of health related telephone surveys to monitor health-related risk behaviors,
chronic health conditions, and use of preventive services of the US residents. In order to conduct the BRFSS, states obtain samples of telephone numbers from CDC.
Household sampling requires interviewers to collect information on the number of adults living within a residence and then select randomly from all eligible adults. Cellular telephone
respondents are weighted as single adult households.This survey was conducted from 2015 to 2022.
The telephonic survey was conducted in the following areas of United States of America:
'Pennsylvania', 'South Dakota', 'Idaho', 'Maryland', 'Wisconsin' ,'Iowa','Oklahoma' ,'Arizona', 'Ohio', 'South' ,'Nevada' ,'Georgia' ,'Northeast', 'Colorado', 'Oregon','Arkansas',
'New York',United States, DC & Territories', 'Puerto Rico', 'Guam' ,'Kansas','Washington', 'Vermont', 'Hawaii', 'District of Columbia', 'Alaska','New Hampshire', 'Montana', 'New Mexico',
'Alabama', 'Louisiana' ,'Kentucky','Utah', 'New Jersey' ,'Tennessee', 'Maine' ,'Texas', 'West Virginia', 'Mississippi', 'Rhode Island', 'Virginia' ,'Nebraska' ,'California', 
'Illinois' ,'Connecticut' ,'North Dakota', 'Massachusetts', 'Florida','South Carolina' ,'North Carolina', 'Wyoming', 'West', 'Midwest', 'Michigan',Virgin Islands', 
'Missouri' ,'Delaware', Minnesota', 'Indiana'.The participants answered 39 questions according to that classified in 7 classes i.e Caregiving,
 Cognitive Decline,Mental Health,	Nutrition/Physical Activity/Obesity, Screenings and Vaccines,Smoking and Alcohol Use,and Overall Health	.
 Data Preprocessing:
 The dataset contains 284142 instances and 31 columns.Out of whichonly 6 were numerical and the rest were catagorical.
 I have done the data preprocessing by handling the missing values by removing/imputing 0/mean/median/mode.There were no duplicates.
 Handled the outliers by using IQR method and percentile method.Encoding, splitting,and feature selection were also done.
 Out of the 31 feature I selected only 11 for furthur analysis.Highly correlated columns were omitted.
 Model Building:
 While model building ,as the data showed inconsistancy I used SMOTE,Pipeline and built models in Logistic Regression,Ridge Classifier,Random Forest Classifier,Gradient Boosting Classifier and K-Nearest Neighbors.
 The best model I got is Gradient Boosting Classifier.Did the HyperparameterTuning using Randomised SearchCV and AUC-ROC score.
 Then tested in the unseen data,which is a similar data of earlier years i.e from 2015-2020, built the pipeline models.
 Conclusion:
After all the analysis I came to the conclusion that the patients with poor mental health,cognitive decline and those smoked and used alcohol experienced Alzheimers rather than those had physical activity,ate fruits and vegetables.
Most of the patients  belong to 50-64 years.
Future Work:
Investigate the use of deep learning approaches, such as neural networks, particularly in processing complex patterns in large datasets. Hybrid models that integrate deep learning with traditional machine learning methods could also be explored.
