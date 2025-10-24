# Mobile Price Classification using SVC

This project involves building a **machine learning model to classify mobile phones into different price ranges** using a dataset from Kaggle. The model uses an optimized **Support Vector Classifier (SVC)** with feature scaling and hyperparameter tuning via **GridSearchCV**.

---

##  Dataset

- **Training set:** `train.csv`  
- **Test set:** `test.csv`  
- **Features:** 20 numerical attributes describing mobile specifications  
- **Target:** `price_range` (0: low, 1: medium, 2: high, 3: very high)

---

##  Approach

1. **Exploratory Data Analysis (EDA)**  
   - Checked feature correlations and distribution of target classes.  
   - Visualized top correlated features using pairplots.  

2. **Preprocessing**  
   - Standardized features using `StandardScaler`.  

3. **Modeling**  
   - Used a **Support Vector Classifier (SVC)** in a pipeline.  
   - Hyperparameter tuning with `GridSearchCV` using `StratifiedKFold` (5 folds).  

4. **Evaluation**  
   - Cross-validation (10 folds) on training set.  
   - Evaluated metrics on the test set: accuracy, precision, recall, F1-score, ROC-AUC, log loss, Cohen’s Kappa, Matthew’s correlation coefficient, top-k accuracy.  
   - Plotted confusion matrix, ROC curves, precision-recall curves, and a heatmap for classification report.

---

##  Visualizations

- **Feature Correlation Heatmap**  
- **Top Features Pairplot by Price Range**  
- **Confusion Matrix**  
- **ROC Curves per Class**  
- **Precision-Recall Curves per Class**  
- **Classification Report Heatmap**

---

##  Model Performance

| Metric                            | Value          |
|-----------------------------------|----------------|
| Cross-val mean Acc ± std deviation| 96.56% ± 0.011 |
| Test Accuracy                     | 97.50%         |
| Precision (weighted)              | 97.62%         |
| Recall (weighted)                 | 97.50%         |
| F1 Score (weighted)               | 97.50%         |
| ROC-AUC Score (OvR)               | 99.95%         |
| Log Loss                          | 0.076          |
| Cohen Kappa Score                 | 96.65%         |
| Matthews Correlation Coefficient  | 96.69%         |
| Top-k Accuracy (k = 2)            | 100%           |

---

##  Tech Stack

- **Language:** Python  
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn, joblib  
- **Machine Learning Algorithm:** Support Vector Classifier (SVC)  
- **Tools:** Jupyter Notebook

---

##  How to Run
1. Clone this repository:
   `bash
   git clone https://github.com/<your-username>/mobile-price-classification.git`
   
---

##  Author  

**Lavan kumar Konda**  
-  Student at NIT Andhra Pradesh  
-  Passionate about Data Science, Machine Learning, and AI  
-  [LinkedIn](https://www.linkedin.com/in/lavan-kumar-konda/)
