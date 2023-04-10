# Stroke-Predection
Stroke prediction using healthcare data

Introduction:

This report analyzes healthcare data that predicts whether a patient has had a stroke based on some features such as age, BMI, work type, gender, etc. The data pre-processing techniques have been applied to this dataset, and exploratory data analysis has been conducted to gain insights into the features and the relationships among them.

Data Pre-Processing:

The first step of this analysis is data pre-processing, which is a crucial step in any machine learning model. The dataset contains 5110 records and 12 features. The data types of features are int64, float64, and object. There are no missing values for all the features except for BMI. The BMI feature has 201 missing values, and the missing values have been filled with the mean value of the column. The 'id' column has been dropped from the dataset because it does not contribute to the analysis.

Exploratory Data Analysis:

The second step was to perform exploratory data analysis (EDA) to get insights into the data. We first checked the correlation between the features of the dataset using the clustermap() method of the seaborn library. This method provides a visual representation of the correlation between the features of the dataset. We also plotted boxplots for all the numerical features of the dataset using the boxplot() method of the seaborn library. The boxplots helped us identify the outliers and the distribution of the data. We then plotted a bar graph to see the frequency of strokes in the dataset. We found that the number of individuals who had a stroke was less compared to those who did not have a stroke. We also plotted a count plot to compare the frequency of strokes in males and females. The plot shows that the frequency of strokes in males is higher. Finally, we plotted a count plot to compare the frequency of strokes in individuals who were ever married and those who were not. The plot shows that the frequency of strokes is higher in individuals who were ever married.

Model Selection:

We performed data pre-processing and exploratory data analysis to clean the data, prepare it for analysis and get insights into the data. The dataset was then ready for predictive modeling using machine learning algorithms. The results of the exploratory data analysis can be used to develop machine learning models that can accurately predict the occurrence of strokes in individuals.

Four different machine learning algorithms (logistic regression, random forest, k-nearest neighbors, and SVM) were used for this stroke prediction dataset. The data is split into training and testing sets with 20% of the data being used for testing.

For each algorithm, the model is trained on the training set and the accuracy score is calculated using the test set. The confusion matrix and classification report are also created using the predicted values of the test set. Hyperparameter tuning is performed using GridSearchCV to find the best parameters for the models.

The accuracy score for the Logistic Regression was found to be 95%.
The accuracy score for the Random Forest was found to be 96%.
The accuracy score for the k-nearest neighbors classifier was found to be 95%.
The accuracy score for the SVC classifier was found to be 96%.

Conclusion:

In conclusion, this is a data analysis project on healthcare data using Python. The data is pre-processed to remove null values, and exploratory data analysis is performed to visualize the relationships between different features and the target variable 'stroke'. The analysis shows that there is a significant difference in stroke frequency between genders, with males having a higher incidence of stroke. The analysis also shows that being married and working in private sectors are associated with a higher incidence of stroke. These findings can help healthcare providers identify high-risk patients and take appropriate measures to prevent or manage strokes.
