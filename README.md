# Credit-Card-Default-Prediction
With the advancement of technology, banks have started to use new strategies to improve their market share. They provide various new services to their customers. A credit card is one such service where a customer can use a certain amount of money and then he is supposed to pay it back. To improve their market shares, banks provide credit cards to their customers without checking their backgrounds. Moreover, many customers use their credit cards beyond their repayment capacity, resulting in higher debt accumulation. It is a greater task for banks to identify risky and non-risky customers. In this project, I have built a supervised ML classification model, which can predict risky and non-risky customers. This model can predict the potential defaulters (who fail to repay within a certain period), thereby helping the banks to take necessary actions.

First, we loaded the given dataset and checked for null and duplicated values. There were no null and duplicated values present. Then we changed the column names for clear understanding. We performed exploratory data analysis to draw many inferences from the data. We noted that the dataset was heavily imbalanced, and some imbalance handling methods were necessary. At the end of the exploratory data analysis, we plotted the heatmap to understand the extent of the relationship between different variables. We converted the categorical data into numerical by one hot encoding. We performed the train-test split and trained several models such as Random Forest, Logistic Regression, KNN, and Decision Tree. We used several performance parameters to measure the performance of each model. Further, we implemented SMOTE (Synthetic Minority Oversampling Technique) to deal with the imbalance in the dataset. After analyzing the performance of each model, we drew some conclusions.

•	There was an imbalance in the target variable. It was handled by SMOTE (Synthetic Minority Oversampling Technique).

•	Accuracy is not a good performance parameter in this problem where the data is imbalanced. We cannot classify a defaulter as a non-defaulter by mistake, i.e., we need to keep an eye on the number of false negatives. Hence, recall is a better performance parameter.

•	We have used Random Forest, Logistic Regression, KNN, and Decision Tree algorithms. Amongst these models, the performance of Logistic Regression was quite poor.

•	Logistic Regression had a heavy imbalance in the recall and precision score, which got balanced after implementing smote. It required further hyperparameter tuning.

•	Decision Tree and Random Forest algorithms performed better with and without SMOTE. Random Forest had a recall score of 93% (for class 0), and 83% (for class 1), and Decision Tree had a recall score of 77% (for class 0), and 91% (for class 1).

•	The performance of all models generally got better with SMOTE.

•	Repayment Status in September, Repayment Status in August and Gender were the important features.
