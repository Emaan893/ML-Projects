# ML-Projects
**Project Report**

This document summarizes the work done in all three projects: Customer Churn Prediction, Mall Customer Segmentation, and Credit Card Fraud Detection. Each project helped me understand different machine learning concepts, especially how to handle real-world datasets and how to select the right evaluation metrics.

---

### **Project 1: Customer Churn Prediction**

In this project, the goal was to predict which customers are likely to leave a subscription service. I used different machine learning models such as Logistic Regression, Decision Tree, Random Forest, and XGBoost.

**What I learned:**

* Logistic Regression performed the best on my dataset.
* Churn prediction is important because companies can take action before losing customers.
* This dataset was not highly imbalanced, so accuracy, precision, recall, and F1-score all made sense to evaluate.

**Confusion Matrix Meaning:**
The confusion matrix shows how many customers the model correctly predicted as “stay” or “leave,” and how many it misclassified. It helped me understand which type of error the model made more often—false positives or false negatives.

---

### **Project 2: Mall Customer Segmentation (K-Means Clustering)**

The goal of this project was to group mall customers into clusters based on features such as income and spending score. This was an **unsupervised learning** task, so there were no labels.

**What I learned:**

* K-Means helps businesses understand different types of customers.
* Choosing the right number of clusters is important (Elbow Method helped).
* Clustering is not about accuracy or recall since there are no true labels. The goal is only to find meaningful groups.

**Outcome:**
I successfully grouped customers into logical clusters such as:

* High income, high spenders
* Low income, low spenders
* Young social shoppers
  These clusters can help in targeted marketing.

---

### **Project 3: Credit Card Fraud Detection (Imbalanced Classification)**

This was the most challenging project because the dataset was extremely imbalanced. Almost all transactions were normal, and only a very small number were fraud.

**Why Accuracy is a BAD Metric Here:**
Accuracy becomes misleading because even if a model predicts “normal” for every transaction, it will still show around **99.8% accuracy**. But the model would actually be *useless* because it missed the fraud cases.

In real-world fraud detection, **missing a fraud (False Negative)** is much more dangerous than predicting something as fraud incorrectly (False Positive).
That's why **Recall** is the most important metric.

**What the Confusion Matrix Means:**

* **True Negative (TN):** Normal transactions correctly identified
* **True Positive (TP):** Fraud transactions correctly detected
* **False Negative (FN):** Fraud that the model failed to detect (worst case)
* **False Positive (FP):** Normal transaction marked as fraud

In my results, the recall for class 1 (fraud) was around **0.74**, which means the model caught 74% of the fraud cases. This is acceptable for an imbalanced dataset but still leaves room for improvement.

**What I Learned About Imbalanced Data:**

* Accuracy is useless when one class dominates the dataset.
* Oversampling, undersampling, or anomaly detection can help.
* Models like Random Forest and XGBoost generally perform better than simple algorithms.
* The confusion matrix tells the real story, not accuracy.
* In fraud detection, we must prioritize **recall**, not accuracy.

---

### **Overall Reflection**

Working on these three projects helped me understand the difference between balanced, imbalanced, and unlabeled datasets. I learned that evaluation metrics must be chosen according to the problem. I also gained confidence in model training, EDA, dealing with imbalance, and interpreting confusion matrices. These projects gave me practical experience similar to real-world data problems.

---

**End of Report**
