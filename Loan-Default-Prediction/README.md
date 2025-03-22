# Loan Default Prediction – PCA & Logistic Regression  

## Dataset  
 **[Loan Data (Google Drive)](https://drive.google.com/drive/folders/1I3H-8KGHDni2CE0t1b_mSAlJ78aQb9iL?usp=sharing)**  
This dataset contains **160 features** related to borrower financials, loan applications, and repayment behavior.  

## Project Overview  
This project explores how **machine learning can improve loan approval decisions** while balancing **accuracy and efficiency**.  

Using **Principal Component Analysis for dimensionality reduction** and **Logistic Regression**, I analyzed how reducing features impacts **predictive power**.  

### **Key Business Questions:**  
1. Can machine learning improve loan approvals?  
2. Does PCA affect prediction accuracy?  
3. Which factors best predict loan repayment?  
 
---

## Results & Insights  

| Model | AUC Score | Accuracy | Best Use Case |
|--------|----------|-----------|----------------|
| **Full Model (160 Features)** | **0.95** | Best accuracy | Best for high-risk loan detection |
| **PCA (100 Features)** | **0.94** | More efficient | Balance of speed & accuracy |
| **PCA (30 Features)** | **0.94** | Good trade-off | Compressed, but still useful |
| **PCA (10 Features)** | **0.68** | Unreliable | Loses key predictive signals |

1. **Best Model:** Full dataset (160 features) → Most accurate but computationally heavy  
2. **Best Trade-Off:** PCA (100 & 30 features) → Faster while maintaining strong predictions  
3. **Worst Model:** PCA (10 features) → Loses too much important information  

---
## Assignment Requirements  
*(This project was completed as part of a university course on applied machine learning. The following is a reworded summary of the original assignment instructions, included for context and academic transparency.)*

In this individual project, I explored how dimensionality reduction affects predictive performance in the context of loan default prediction. The dataset used contained 160 features related to loan applications, borrower profiles, and repayment behavior.

THe objective was to understand how reducing the number of features using **Principal Component Analysis (PCA)** impacts the accuracy and efficiency of a **Logistic Regression** model when predicting loan repayment status.

- Used a cleaned version of the **Lending Club loan dataset**, with 160 input features.
- Set `'loan_status'` as the **target variable**, with the remaining features used for prediction.
- Applied **Min-Max Scaling** to standardize data before modeling.
- Performed **Principal Component Analysis (PCA)** to reduce feature dimensions to:
  - **100 components**
  - **30 components**
  - **10 components**
- Trained **four Logistic Regression models**:
  1. Full dataset (160 features)
  2. PCA with 100 components
  3. PCA with 30 components
  4. PCA with 10 components
- Evaluated models using:
  - **Precision**
  - **Recall**
  - **F1-score**
  - **ROC curves** and **AUC scores**
- Plotted a **Screen Plot** to visualize how much variance was captured at each PCA level.

---

## What I Learned from This Project  

- **Machine learning isn’t just about accuracy—it’s about balancing efficiency and interpretability.**  
- **PCA can reduce complexity**, but too much dimensionality reduction weakens predictions.  
- **For real-world applications, we need models that are fast, fair, and explainable.**  

---

## Tools & Techniques Used  
- **Python** (Pandas, NumPy, Scikit-Learn, Matplotlib)  
- **Machine Learning** (PCA, Logistic Regression, Feature Scaling)  
- **Evaluation Metrics** (Precision, Recall, F1-score, AUC-ROC)  
- **Business Analytics** (Loan Risk Assessment)  

---
