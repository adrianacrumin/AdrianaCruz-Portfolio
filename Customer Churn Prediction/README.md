# Customer Churn Prediction - Classification Models & SMOTE 

## Dataset  
 **[Customer Churn Telecom (Google Drive)](https://drive.google.com/file/d/1zyHrkF1jCUp-2irwohVpYVMMMX7EdSFo/view?usp=sharing)**  
This dataset contains **demographic, account, and service information** for telecom customers, along with whether or not they churned (canceled service).  


## Project Overview  
This project explores how **machine learning can help telecom companies reduce churn** by identifying customers likely to leave.  

Using three classification models and **SMOTE** to handle class imbalance, I analyzed how each model performed and whether rebalancing the data led to better predictions.  

### **Key Business Questions:**  
1. Can machine learning help predict which customers are at risk of churning?  
2. Which classification model performs best on this task?  
3. Does class imbalance impact model performance?  
4. Can SMOTE improve prediction accuracy for minority classes? 
 
---

## Results & Insights  

| Model                      | Data        | AUC Score | Best Use Case                    |
|----------------------------|-------------|-----------|----------------------------------|
| Logistic Regression        | Imbalanced  | High      | Best balance of accuracy & recall|
| MLP Classifier (Neural Net)| Imbalanced  | High      | Captures nonlinear patterns well |
| Decision Tree              | Imbalanced  | Moderate  | Fast & interpretable             |
| Logistic Regression        | SMOTE       | Improved  | Better at identifying churners   |
| MLP Classifier             | SMOTE       | Improved  | Stronger on balanced data        |


1. **Best Model:** Logistic Regression (with or without SMOTE) – interpretable and consistent  
2. **Best for Recall:** MLP Classifier with SMOTE – picks up more true churners  
3. **Worst Scenario:** Any model without addressing imbalance – high accuracy, low recall


---
## Assignment Requirements  
*(This project was completed as part of a graduate-level machine learning course. The following is a reworded summary of the original assignment instructions, included for context and academic transparency.)*

The objective of this project was to explore **classification models** for **predicting customer churn** and to evaluate the effect of **class imbalance** on performance.  

- Cleaned and preprocessed the telecom churn dataset:
  - Encoded binary variables and performed one-hot encoding
  - Handled "No internet service"/"No phone service" responses
- Split the dataset into train/validation/test sets using stratified sampling
- Trained **three models**:
  1. Logistic Regression  
  2. Decision Tree  
  3. MLP Classifier (Neural Network)  
- Evaluated using:
  - **Precision**
  - **Recall**
  - **F1-score**
  - **ROC curves** and **AUC scores**
  - **Precision-Recall Curves**
- Handled **class imbalance** using **SMOTE**
- Retrained Logistic & MLP models after applying SMOTE
- Compared model performance before and after balancing the data

---

## What I Learned from This Project  

- **Accuracy alone is misleading in imbalanced datasets** — recall and AUC are critical.  
- **SMOTE significantly improves model fairness** by allowing better detection of churners.  - **Logistic Regression remains a strong baseline**, especially for business use cases that need transparency.  
- **Neural nets (MLP)** can outperform traditional models with proper balancing and tuning. 
- **Data preprocessing** and feature encoding have a huge impact on model quality.

---

## Tools & Techniques Used  
- **Python** (Pandas, NumPy, Scikit-Learn, Matplotlib)  
- **Machine Learning** (Decision Tree, Logistic Regression, MLP Classifier (Neural Networks)  
- **Evaluation Metrics** (Precision, Recall, F1-score, AUC-ROC, PR Curve)  
- **Business Analytics** Customer Churn Risk Prediction & Retention Strategy 

---

