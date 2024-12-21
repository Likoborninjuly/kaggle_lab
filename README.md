# kaggle_lab
Detailed comparison of K-Nearest Neighbors (KNN) and the other five algorithms:

| Algorithm               | Accuracy | Precision (Neg/Pos) | Recall (Neg/Pos) | F1-Score (Neg/Pos) |
|-------------------------|----------|----------------------|-------------------|---------------------|
| K-Nearest Neighbors     | 0.794    | 0.74 / 0.81         | 0.55 / 0.91      | 0.63 / 0.86         |
| Multinomial Naive Bayes | 0.800    | 0.89 / 0.78         | 0.43 / 0.97      | 0.58 / 0.87         |
| Decision Tree           | 0.923    | 0.92 / 0.93         | 0.84 / 0.96      | 0.87 / 0.94         |
| Random Forest           | 0.916    | 0.95 / 0.90         | 0.78 / 0.98      | 0.86 / 0.94         |
| Support Vector Machine  | 0.868    | 0.92 / 0.85         | 0.64 / 0.97      | 0.76 / 0.91         |
| Logistic Regression     | 0.866    | 0.96 / 0.84         | 0.61 / 0.99      | 0.74 / 0.91         |

Key Observations
1. Accuracy
KNN achieves an accuracy of 79.4%, which is lower than the other algorithms.
Decision Tree (92.3%) and Random Forest (91.6%) outperform KNN significantly, indicating these tree-based models handle this dataset more effectively.
2. Precision
For the Neg class, KNN (74%) is outperformed by all other models, especially Random Forest (95%) and Logistic Regression (96%).
For the Pos class, KNN (81%) is comparable to Naive Bayes (78%) but still lower than Decision Tree (93%).
3. Recall
For the Neg class, KNN (55%) is better than Naive Bayes (43%) but falls behind the tree-based models and SVM.
For the Pos class, KNN (91%) performs reasonably well and is comparable to SVM (97%) and Random Forest (98%).
4. F1-Score
For the Neg class, KNN’s F1-Score (63%) is lower than all other models.
For the Pos class, KNN’s F1-Score (86%) is decent but still below Decision Tree (94%) and Random Forest (94%).
Strengths of KNN
Simple and Intuitive: KNN is easy to understand and implement.
Good Recall for Positive Class: KNN achieves a recall of 91%, meaning it effectively identifies positive cases.
No Training Time: KNN doesn’t involve model training, which can be an advantage for small datasets.
Weaknesses of KNN
Low Precision and F1-Score for Negative Class: This indicates that KNN struggles to correctly identify the negative class and has higher false positives.
Low Accuracy Compared to Other Models: Models like Decision Tree and Random Forest outperform KNN significantly in terms of overall accuracy.
Sensitive to Noisy Data: KNN is heavily influenced by outliers or noisy data, which might explain its lower performance.
