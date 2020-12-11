# Unit 11—Risky Business

![risky_business](Images/risky_business.jpg)


## Credit Risk Resampling Techniques

summary_results-part1
![summary_results-part1](Images/summary_results-part1.jpg)

The table above shows a discrepancy between the calculated numbers and the numbers already in the starter code. 

Using the starter code numbers, the model with the highest accuracy score is the random over sampler followed by SMOTE (Synthetic Minority Oversampling Technique). The best recall is also for these two models. Lastly, the geometric mean is also highest for the random over sampler model and the SMOTE has a similar score than the SMOTEENN (SMOTE + Edited Nearest Neighbor)

The accuracy of the first two might be driven by the overfitting that those models tend to do when they increase the size of the minority class, in this case, the high risk loans. 


## Credit Risk Ensemble 

![summary_results-part2](Images/summary_results-part2.jpg)

Based on the table above, the Easy Ensemble Classifier has the highest accuracy model, recall score and geometric mean, making in the model of choice for LendingClub data. 

![Feautres_Importance](Images/Feautres_Importance.png)

The top 3 features are total_rec_prncp, total_pymnt, total_pymnt_inv followed by other metrics that seem counterituitive. 

When comparing this to the features in the starter code, there seems to be a discrepancy. The starter code, shows loan_amnt, int_rate and instalrmment followed by annual_inc, dti, delinq_2yrs. These features are more closely related to loan performance than the ones identified by the model I ran. 



## Appendix - Credit Risk Resampling Techniques - Classification Reports

### Oversampling
![random_over_sampler_class_report](Images/random_over_sampler_class_report.jpg)

#### Naive Random Sampling

#### SMOTE Oversampling
SMOTE_class_report
![SMOTE_class_report](Images/SMOTE_class_report.jpg)

### Undersampling

#### Cluster Centroids
![under_sampler_class_report](Images/under_sampler_class_report.jpg)

### Combination (Over and Under) Sampling

#### SMOTEENN 
![SMOTEENN](Images/SMOTEENN.jpg)


## Appendix - Credit Risk Ensemble - Classification Reports

#### Balanced Random Forest Classifier
![balanced_random_forest_class_report.png](Images/balanced_random_forest_class_report.png.jpg)

#### Easy Ensemble Classifier
![EEC_class_report](Images/EEC_class_report.jpg)