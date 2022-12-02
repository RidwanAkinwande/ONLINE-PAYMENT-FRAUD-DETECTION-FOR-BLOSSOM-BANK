# ONLINE-PAYMENT-FRAUD-DETECTION-FOR-BLOSSOM-BANK

Because of technological advancements, the rise in online transaction fraud has become a big concern for banks and financial institutions in today's world. The goal of this project is to build a Machine Learning model for Blossom Bank to predict online payment fraud.

The Bloom Bank dataset is imbalanced because Fraudulent transaction (1) has a relatively low 0.11%, and the Non-Fraudulent transaction (0) has 99.9%, resulting in an accuracy score of 99% for all models tested in this project.

Could accuracy be the best metric to use to evaluate the models?

No, because the models predicted only 0.11% incorrectly: Majority of Bloom Bank online transactions were misclassified as non-fraudulent. As a result, the percentage of correct predictions is 99%. The problem here is that 99% accuracy sounds like a great result, but the models perform quite poorly.

To summarize, when the dataset is imbalanced, accuracy is not a good metric to utilize.

Let's have a look at the Precision and Recall for each model.

The precision of Logistic Regression is 0.56 and the recall is 0.32. The precision of KNeighbors is 0.80 and the recall is 0.54. The precision of Decision Tree is 0.82 and the recall is 0.80. Random Forest, on the other hand, has a precision of 0.98 and a recall of 0.72. Because our model is designed to predict type of fraudulent transactions from the dataset. It can be shown that the Random Forest model has the highest precision (98%). Is this to say that Random Forest is the best model? Perhaps we might investigate further by examining the F1 score for each model.

The F1 score is the metric in which we are most interested. The goal is to demonstrate its value in modeling with imbalanced datasets. The final F1 score of the Logistic Regression was 41% and KNeighbors was 64%: we can't be satisfied with this score because the percentages were so low. The Decision Tree had an F1 score of 81%, whereas the Random Forest had an F1 score of 83%. This demonstrates that the Decision Tree and Random Forest have a small margin, which, while far from perfect, is a significant improvement over the Logistic Regression and KNeighbor models.

This is crucial information that we could not have obtained using accuracy as a metric because all of the models' accuracy is the same.

Conclusion

The F1 score was used as a model performance metric in this project. When working on classification models with an imbalanced dataset, the F1 score becomes extremely useful.

The F1 score, as we've seen, combines precision and recall into a single metric.

Accuracy can be quite deceiving because it offers a high score to a bad model. The F1 score is far superior in predicting the performance of a machine learning model.

As a result, the Random Forest model with F1 score of 83% performed best, which will assist Blossom Bank in keeping track of any suspicious transactions. Hence, Blossom Bank should be more concerned with better results on True Positives.

