# Loan Default Prediction – PCA & Logistic Regression  

## Dataset  
 **[Loan Data (Google Drive)](https://drive.google.com/drive/folders/1I3H-8KGHDni2CE0t1b_mSAlJ78aQb9iL?usp=sharing)**  
This dataset contains **160 features** related to borrower financials, loan applications, and repayment behavior.  

## Project Overview  
This project explores how **machine learning can improve loan approval decisions** while balancing **accuracy and efficiency**.  

Using **Principal Component Analysis for dimensionality reduction** and **Logistic Regression**, I analyzed how reducing features impacts **predictive power**.  

### **💡 Key Business Questions:**  
✔ Can machine learning improve loan approvals?  
✔ Does PCA affect prediction accuracy?  
✔ Which factors best predict loan repayment?  
 
---

## Results & Insights  

| Model | AUC Score | Accuracy | Best Use Case |
|--------|----------|-----------|----------------|
| **Full Model (160 Features)** | **0.95** | ✅ Best accuracy | Best for high-risk loan detection |
| **PCA (100 Features)** | **0.94** | ✅ More efficient | Balance of speed & accuracy |
| **PCA (30 Features)** | **0.94** | ✅ Good trade-off | Compressed, but still useful |
| **PCA (10 Features)** | **0.68** | ❌ Unreliable | Loses key predictive signals |

✔ **Best Model:** Full dataset (160 features) → Most accurate but computationally heavy  
✔ **Best Trade-Off:** PCA (100 & 30 features) → Faster while maintaining strong predictions  
✔ **Worst Model:** PCA (10 features) → Loses too much important information  

---
## Assignment Requirements  
(*For academic transparency, these are the original instructions.*)  

## 1. PCA
In this problem we will be applying PCA on the Lending Club loan dataset. A simplified version of the dataset with reduced number of samples. Please use the dataset given in the file named `loan.csv`.

### **1. Data Preprocessing**  
- Select `'loan_status'` as the target variable (`y`), with all other features as `X`.  
- Split data into **training (75%) and testing (25%)** sets.  
- Apply **Min-Max Scaling** to standardize features.  
- Ensure `X` has **160 features** after preprocessing.  

### **2. Dimensionality Reduction with PCA**  
- Apply PCA to reduce features to **100, 30, and 10 principal components**.  
- Print the **percentage of variance captured** at each level.  
- Plot a **Scree Plot** to visualize variance retention.  

### **3. Logistic Regression Models**  
- Train **four logistic regression models**:  
  1. **Full dataset (160 features)**  
  2. **PCA-reduced dataset (100 features)**  
  3. **PCA-reduced dataset (30 features)**  
  4. **PCA-reduced dataset (10 features)**  
- Evaluate performance using **Precision, Recall, F1-score**.  

### **4. Model Evaluation via ROC Curve**  
- Plot **ROC curves** for all models.  
- Compute **AUC scores** to compare classification performance.  

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
