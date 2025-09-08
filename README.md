# Predicting-Mortality-of-Heart-Failure-Patients

This project aims to develop a machine learning model to predict the mortality risk of patients with heart failure using their clinical records. By leveraging a 

Logistic Regression algorithm, this model serves as a clinical decision support tool, helping to identify high-risk patients who may require early intervention.



Dataset Overview 🩺
The analysis is based on a clinical records dataset containing information from 

299 patients.



Total Features: 13.



Data Quality: The dataset is 100% complete, with no missing values.

Feature Composition: The features are categorized into:


7 Numerical Features (e.g., age, platelets, serum sodium).



5 Binary Features representing various health conditions.

1 Target Variable (DEATH_EVENT).

⚙️ Data Processing & Modeling Pipeline
Data Preprocessing
To prepare the data for analysis, the following steps were taken:


Feature Scaling: StandardScaler normalization was applied to all 7 numerical features to standardize their ranges.



Train-Test Split: The dataset was divided into a training set (80%) and a testing set (20%) using stratification to maintain the same proportion of outcomes in both splits. This resulted in 239 training samples and 60 testing samples.


Model Implementation
A 

Logistic Regression model was implemented for this binary classification task. The model takes 12 clinical variables as input and uses a 


Sigmoid function to calculate the probability of mortality, outputting a prediction of either 0 (survives) or 1 (deceased).




📊 Model Performance
The model achieved strong predictive performance, demonstrating its effectiveness in distinguishing between high-risk and low-risk patients.

Key Metrics
Metric	Score
Accuracy	
81.67% 


AUC Score	
86.14% 

Precision	
78.57% 

Recall (Sensitivity)	
57.89% 

F1-Score	
66.67% 


Export to Sheets
Confusion Matrix Analysis
The confusion matrix provides a deeper insight into the model's predictions on the test set of 60 samples:


True Positives: 11 (Correctly predicted as deceased).



True Negatives: 38 (Correctly predicted as survivors).



False Positives: 3 (Incorrectly predicted as deceased).




False Negatives: 8 (Incorrectly predicted as survivors).


The model shows a high 

Specificity of 92.7%, indicating an excellent ability to identify surviving patients correctly. However, the 



Sensitivity (Recall) of 57.9% suggests there is potential for improvement in identifying patients at risk of mortality.


💡 Conclusion & Future Directions
Conclusion
The Logistic Regression model is a successful tool for predicting heart failure mortality, achieving an 

accuracy of 81.67% and an AUC score of 86.14%. This demonstrates a strong ability to discriminate between patients who are likely to survive and those who are not, making it a valuable asset for clinical risk assessment.




Future Work
To further enhance the model's predictive power, the following steps are proposed:


Advanced Algorithms: Explore more complex models like ensemble methods (e.g., Random Forest, Gradient Boosting) and neural networks.


Feature Engineering: Incorporate additional clinical markers and patient history data to provide the model with more context.


Clinical Validation: Validate the model's performance on larger, multi-center datasets to ensure its broader applicability.


Clinical Integration: Develop a user-friendly interface to integrate the model into clinical workflows for real-time decision support.
