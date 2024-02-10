# Predicting-Income-with-Python-Classification-Algorithms
 
##Overview
This task focused on using classification algorithms to predict income levels in a selected demographic, utilizing Python's robustness and Azure MLD's cloud-based platform. The analysis was performed on the Adult Dataset from the UCI Machine Learning Repository. This dataset, ideal for classification tasks, contains rich attributes like race, gender, marital status, and occupation, aimed at predicting whether an individual's annual income exceeds $50,000. The goal was to gain insights into income level determinants and broader socio-economic dynamics.

##Data Cleaning and Transformation
The data processing involved handling missing values, detecting outliers, and encoding data. Missing values, identified as question marks, were addressed using mode imputation for categorical variables and KNN imputation for more diverse variables. The dataset had a substantial number of outliers, managed by winsorizing numerical columns and using robust modeling methods. Categorical variables were transformed using One Hot Encoding, and numerical features were standardized using StandardScaler from sklearn. The processed data was then split into training and testing sets.

##EDA
The dataset underwent further exploration using Chi-Square and Correlation Matrix. Key findings include a modest positive correlation of 'age' with 'education-num' and 'capital-gain', and 'education-num' with 'hours-per-week'. Chi-Square tests revealed strong associations between 'income level' and variables like 'workclass', 'education', 'marital-status', and others. Three classification algorithms (Random Forest, KNN, Decision Tree) were applied, with Random Forest showing a good performance score of approximately 85.7% accuracy and a high ROC-AUC score, indicating effective class separation and robustness against overfitting.

##Recommendation
The Random Forest classifier is recommended for predicting income levels due to its high accuracy, balanced precision and recall, and capability to handle complex relationships between features. Its strong generalization capability and robustness to overfitting make it suitable for real-world deployment. However, it might require more computational resources. Decision Tree could be a secondary option if interpretability or computational resources are constraints. Further improvements could be explored through hyperparameter tuning, feature engineering, handling class imbalance, and ensemble methods.

##Classification Algorithm - Results of Analysis
The analysis using Random Forest, KNN, and Decision Tree algorithms yielded distinct insights:

###Random Forest: Demonstrated an accuracy of approximately 85.7% with a high ROC-AUC score of 0.9065, indicating effective class separation and robustness against overfitting. It was particularly strong in predicting the majority class (income ≤ $50k), with higher precision for this class and a reasonable balance between precision and recall.

###KNN (k-Nearest Neighbors): Showed an accuracy of about 77.7%, with a fair ability to classify the minority class (income > $50k). However, it had a lower precision and recall for this class, indicating some challenges in accurately classifying higher income levels.

###Decision Tree: Achieved an accuracy of 80.44%, with moderate precision and a fair recall rate for the positive class (income > $50k). It showed a better performance in identifying the negative class (income ≤ $50k) compared to the positive class.
