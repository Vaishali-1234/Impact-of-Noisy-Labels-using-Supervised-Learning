#  Impact of Noisy Labels using Supervised Learning

Understanding how noisy (incorrect) labels affect the performance of supervised learning models. This project experiments with multiple machine learning algorithms on the **SMS Spam Collection Dataset**, injecting varying levels of label noise (10% to 50%) and observing performance degradation.

---

## 📂 Dataset

**Source**: [SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)  
**Attributes**:  
- `label`: spam / ham  
- `text`: SMS message content

---

## 🎯 Objectives

- 🧠 Train & Evaluate Multiple ML Models  
- 🔀 Simulate Label Noise by Randomly Flipping True Labels  
- 📉 Track Impact on Accuracy, Precision, Recall, and F1-Score  
- 📊 Visualize Performance Degradation as Noise Increases  

---

## 🤖 Algorithms Used

- Logistic Regression  
- Support Vector Machine (Linear SVC)  
- Random Forest Classifier  

---

## 📈 Results Snapshot

| 🔁 Noise Level | Logistic Regression | SVM | Random Forest |
|---------------|---------------------|-----|----------------|
| 0% (No Noise) | ✅ 97.10%            | 96.93% | 🥇 97.05%     |
| 10%           | 94.75%              | 94.40% | 95.01%        |
| 30%           | 91.20%              | 89.88% | 93.02%        |
| 50%           | 86.30%              | ⚠️ 83.15% | ✅ 88.64%    |

- ✅ **Best Model (Most Robust)**: Random Forest  
- ⚠️ **Most Sensitive to Noise**: SVM  

---

## 🧠 Key Observations

- Model performance drops consistently with increasing label noise.
- Random Forest was most robust, handling noise better than linear models.
- SVM’s performance declined sharply with noisy data.
- Highlights the critical importance of **clean, reliable data** in real-world ML applications.

---

## 🛠️ Tools & Libraries

- Python  
- Scikit-learn  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Tqdm (for progress bars)

---

