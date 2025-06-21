# 🚨 Credit Card Fraud Detection

This project aims to detect fraudulent credit card transactions using supervised machine learning techniques.  
We applied *sampling strategies* to tackle data imbalance and used a *Decision Tree Classifier* for classification.

---

## 📂 Dataset Information

- Total Records: *555,721*
- Target Column: is_fraud (0 = Genuine, 1 = Fraud)
- Data has heavy class imbalance.

---

## ⚙ Tools & Libraries Used

- Python 🐍
- Pandas, NumPy
- Scikit-learn (Sklearn)
- Matplotlib, Seaborn

---

## 📌 Steps Followed

1. *Data Cleaning*  
   - Removed irrelevant columns (merchant, street, etc.)  
   - Checked for null values and datatypes

2. *Feature Engineering*  
   - Applied encoding on category  
   - Standardized numerical features using StandardScaler

3. *Handling Imbalance*  
   - Used *Random Under Sampling*  
   - Also tried *SMOTE (Synthetic Minority Oversampling Technique)* for comparison

4. *Model Building*  
   - Trained using *Decision Tree Classifier*  
   - Tuned and compared performance on both sampling methods

5. *Evaluation*  
   - Used Confusion Matrix, F1 Score, Precision, Recall, Accuracy

---

## 📈 Model Performance (Best Result)

Using *Random Under Sampler + Decision Tree*:
- 🔹 Accuracy: *99.4%*
- 🔹 F1 Score: *94.7%*
- 🔹 Recall: *94.3%*

> Fraud detection focuses on *maximizing Recall* – catching frauds is more important than mislabeling genuine transactions.

---

## ✅ Conclusion

- Undersampling gave better recall and more reliable fraud detection.
- Precision is slightly compromised, but *recall is the key*.
- The model performed exceptionally well compared to typical benchmarks.

---

## 💻 How to Run

1. Clone the repo
2. Open Credit_card_fraud.ipynb in Jupyter Notebook
3. Run all cells step by step
