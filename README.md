# Predictive Modeling for Student Enrollment
This project uses machine learning to predict student outcomes (Graduate, Dropout, Enrolled) based on academic, demographic, and socio-economic data. The objective of this project is to reduce dropouts by identifying students at high risk at an early stage of their academic path, using machine learning models. The dataset used is from [UCI Machine Learning Repository](https://doi.org/10.24432/C5MC89), it contains 36 features including information known at the time of student enrollment. 

The methods used for **data preparation** included encoding categorical variables, standardizing numeric values and using dimensionality reduction techniques to simplify the dataset and improve computational efficiency. PCA reduced features from 31 to 18 (90% variance retained). 

I also performed **Exploratory Data Analysis (EDA)**, making KDE Plots, Violin plots and a Correlation heatmap to better visualize feature distributions, outliers and correlations with the target variable. 

The **machine learning models** trained included: Naive Bayes, Logistic Regression, Decision Tree, KNN and SVM, which were evaluated on accuracy, precision, recall, and F1-score. An **ensemble model** combining the best performing models (SVM, Logistic Regression and KNN) was implemented using a majority voting scheme, achieving a final accuracy of 75%. The ensemble model also achieved an F1-score of 0.78, indicating balanced performance across all classes.

10-Fold Cross-Validation was used to ensure model robustness and prevent overfitting. Cross-validation accuracy was consistent across all folds. Lastly, permutation importance was used to understand the key factors that influence student dropouts, which were discovered to be: age at enrollment, 2nd semester grades, and daytime attendance. 

This project demonstrates how data-driven insights and machine learning can empower educational institutions to proactively address student dropouts and improve academic outcomes.
