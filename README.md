# Impact-of-Noisy-Labels-using-Supervised-Learning

Understanding the Impact of Noisy Labels on Supervised Learning
A machine learning project focused on evaluating how label noise affects model accuracy and robustness. This project compares multiple classification algorithms on the SMS Spam dataset under increasing levels of label corruption (10% to 50%) and visualizes performance degradation.

📊 Dataset
Source: SMS Spam Collection Dataset (https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)
Attributes: Label (ham/spam), SMS Text

🎯 Objectives

Train and Compare ML Models: Logistic Regression, Support Vector Machine (SVM), Random Forest

Label Noise Injection: Flip labels randomly to simulate mislabeled data

Performance Analysis: Track model accuracy, precision, recall, and F1 score with increasing noise

Visualization: Graph model performance as noise increases

🤖 Algorithms Used

Logistic Regression
Support Vector Machine (LinearSVC)
Random Forest

📈 Results (Sample - May Vary by Run)
Noise Level	Logistic Regression	SVM	Random Forest
0%	97.10% ✅	96.93%	97.05%
10%	94.75%	94.40%	95.01%
30%	91.20%	89.88%	93.02%
50%	86.30%	83.15%	88.64% ❗
✅ Most Robust Model: Random Forest
📉 Most Sensitive to Noise: SVM

🔍 Observations

Model robustness decreases with increasing label noise.
Random Forest handled noise more gracefully than linear models.
Emphasizes the importance of label quality in real-world machine learning tasks.
