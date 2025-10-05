# Mobile Price Classification using SVC

This project applies **Support Vector Classifier (SVC)** to the **Mobile Price Classification dataset** from Kaggle.  
Since the official test set had no labels, the train set  was manually split into training and testing sets to evaluate the model’s performance.  
The goal of this project is to accurately classify mobile phones into their respective price ranges using ML techniques.

---

## Results Summary

|  Metric                  |  Score           |
|:-------------------------|:----------------:|
| **Cross-Val Mean ± Std** | **94.5% ± 0.02** |
| **Best Cross-Val Score** | **94.93%**       |
| **Test Accuracy**        | **97.25%**       |
| **Precision**            | **97.46%**       |
| **Recall**               | **97.25%**       |
| **F1 Score**             | **97.26%**       |

---

##  Key Features
- ✅ Used `train_test_split` with a **test ratio of 0.2** to evaluate performance.  
- ✅ Applied **StandardScaler** to normalize the feature data for better SVC convergence.  
- ✅ Implemented **GridSearchCV** and **StratifiedKFold** to tune hyperparameters and ensure robust evaluation.  
- ✅ Trained the final model using the best parameters found via Grid Search.  
- ✅ Predicted on the split test set and evaluated performance metrics.  
- ✅ Displayed **Confusion Matrix** and **Classification Report Heatmap** using `seaborn` for visual insights.  
- ✅ Achieved **high accuracy and consistency** across validation folds and test data.  

---

##  Tech Stack
- Python  
- scikit-learn  
- NumPy  
- pandas  
- Matplotlib  
- Seaborn  

---

## 📂 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/mobile-price-classification.git
