# UNP_ML_CLASSIFICATION_PROJECT_AIRLINE_PASSENGER_SATISFACTION_USING_PYTHON

I completed this project as part of my Data Science and Machine Learning Internship with United Network of Professionals (UNP), and it was executed as a collaborative group project.

Project Overview This end-to-end classification project focused on predicting airline passenger satisfaction and identifying the key operational service drivers behind customer experience. Using a survey dataset of 103,904 passenger records across 25 attributes, our team built a binary classifier to distinguish between satisfied and neutral or dissatisfied passengers while uncovering actionable business insights.

Data Preprocessing and Feature Engineering During preprocessing, we cleaned the dataset by removing non-predictive identifier columns and dropping 310 rows with missing arrival delay values, resulting in 103,594 clean records. All categorical variables, including gender, customer loyalty status, travel type, and cabin class, were numerically encoded, and continuous features were standardized for distance-based and linear algorithms.

Exploratory Data Analysis and Multicollinearity Resolution Through exploratory data analysis, we analyzed class balance (56.66% neutral or dissatisfied vs. 43.34% satisfied) and discovered that business class travelers, loyal customers, and business-purpose flyers had significantly higher satisfaction rates. Correlation and Variance Inflation Factor (VIF) testing revealed severe multicollinearity between arrival delay and departure delay (r = 0.965, VIF > 14.7), leading us to drop arrival delay and bring all remaining 21 predictors under a healthy VIF threshold of 3.89.

Machine Learning and Deep Learning Benchmarking We systematically benchmarked 9 classical machine learning algorithms across 5 different train-test splits alongside 10 distinct Artificial Neural Network (ANN) architectures using Adam and SGD optimizers. Tree-based ensemble models consistently outperformed linear models and neural networks, with XGBoost emerging as the top performer at 96.43% test accuracy and 0.9952 ROC AUC, closely followed by Random Forest at 96.22% and our best bottleneck ANN architecture at 95.83%.

Key Business Insights and Conclusion Our analysis demonstrated that online boarding (r = 0.50) and inflight entertainment (r = 0.40) are the strongest service-rating drivers of overall passenger satisfaction, followed by seat comfort and cleanliness. Ultimately, we recommended deploying the XGBoost classifier into production due to its superior predictive accuracy, rapid inference speed, and clear feature interpretability for guiding airline service investments.

GOOGLE COLAB FILE LINK: https://drive.google.com/file/d/1mHxhyUAq2tg5ZfyiwgYcgRrpK-lhuuAv/view?usp=sharing

PROJECT PRESENTATION FILE LINK: https://docs.google.com/presentation/d/1pcz-Bklm1YGFK31Ii0JwNbQY7Hj9yjd8/edit?usp=sharing&ouid=110964033644526735796&rtpof=true&sd=true
