# credit-risk-classification

#Description:

This analysis utilizes various machine learning techniques to train and assess the performance of Logistic Regression Models in determining the creditworthiness of borrowers. These models are trained using different methods, and their performance is compared to identify the superior-performing model. The predictive variables in the model are represented as labels 0 (healthy loan) and 1 (high-risk loan).

In the model construction process, the dataset is divided into features and labels, further segmented into training and testing sets.

Machine Learning Model 1 is constructed by initializing a logistic regression model, training it with the original training sets (X_train, y_train), fitting it to the training data, and utilizing it for generating predictions.

Machine Learning Model 2 is developed by resampling the original training data using the RandomOverSampler module. It involves initializing a logistic regression model, fitting the resampled training sets (X_resample, y_resample) to the model, and generating predictions.
The performance of each model is evaluated based on multiple metrics, including the balance accuracy score, confusion matrix, precision score, recall score, and f1-score in the classification report.

Results:

Machine Learning Model 1:

Model 1, trained on the original data, achieves an accuracy of 94.4% in predicting the two labels. The model excels in predicting healthy loans, with both precision and recall scores of 1.00. However, its performance in predicting high-risk loans can be enhanced. The precision score for high-risk loans stands at 0.87, indicating that only 87% of actual high-risk loans were correctly predicted. The recall score for high-risk loans is 0.89, suggesting that the model identified 89% of all high-risk loans in the dataset.

Machine Learning Model 2:

Model 2, trained on the resampled data, attains an accuracy of 99.6% in predicting the two labels. The model demonstrates proficiency in predicting healthy loans, with precision and recall scores of 1.00. While the precision score for high-risk loans remains at 0.87, the recall score has improved to 1.00. This indicates that the model can now correctly predict all high-risk loans in the dataset.

Summary:

Based on the analysis, it is evident that Model 2 surpasses Model 1 in predicting high-risk loans and achieves an overall higher accuracy in predicting both labels. Specifically, Model 2 attains a relatively high precision in predicting high-risk loans while correctly identifying all high-risk loans in the dataset. This performance is considered commendable in this context. Therefore, it is recommended to utilize Model 2 for identifying high-risk loans and achieving better accuracy in predicting labels.