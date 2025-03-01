# Loan Default Prediction – PCA & Logistic Regression  

## Project Overview  
This project explores **loan default prediction using Principal Component Analysis (PCA) and Logistic Regression**. The goal is to evaluate how dimensionality reduction affects **model accuracy and interpretability**, helping lenders make **smarter risk assessments** while maintaining efficiency.  

By applying **PCA** to reduce the number of features and training **four logistic regression models**, we analyze the trade-off between **computational efficiency and predictive power** in financial modeling.  

---

## Business Purpose  
Lending institutions must **accurately identify high-risk loans** to minimize defaults while maximizing approved loans. However, using **too many features** in a predictive model can lead to **higher complexity, slower processing, and potential overfitting**.  

This project answers key business questions:  
✔ **Can machine learning improve loan approval decisions?**  
✔ **Does reducing feature dimensions via PCA affect model performance?**  
✔ **Which factors most strongly predict loan repayment behavior?**  

By balancing **predictive accuracy with computational efficiency**, this project supports **data-driven lending strategies**, reducing financial risk while maintaining business growth.  

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

## Key Findings & Business Takeaways  
| Model | AUC Score | Accuracy | Best Use Case |
|--------|----------|-----------|----------------|
| **Full Model (160 Features)** | **0.95** | ✅ **Best Model** | High accuracy & recall |
| **PCA (100 Features)** | **0.94** | ✅ **Efficient Model** | Reduces complexity but performs well |
| **PCA (30 Features)** | **0.94** | ✅ **Good Balance** | Slightly compressed, still useful |
| **PCA (10 Features)** | **0.68** | ❌ **Unreliable** | Loses too much information |

**Business Takeaway:**  
- **Full Model (160 Features)** is ideal for **accuracy-driven loan risk assessment**.  
- **PCA (100 & 30 Features)** provides **a more efficient model while maintaining strong predictive power**.  
- **PCA (10 Features) is too compressed** and removes too much important information for real-world use.  

---

## What I Learned from This Project  

Before this project, I thought machine learning models were all about getting the highest accuracy possible. Now, I realize that in business, it's about balancing predictive power with practical use. Lenders don’t just need a good model—they need something interpretable, efficient, and fair. This assignment helped me see how dimensionality reduction like PCA can be a useful tool, but only when applied carefully. 

Through **PCA and Logistic Regression**, I saw how reducing features can improve efficiency but may also lead to **loss of key predictive signals**—a crucial trade-off in real-world consumer analytics.  

More importantly, I learned that **machine learning isn’t just about accuracy—it’s about making models practical for business decisions**. In lending, risk assessment requires **transparency, efficiency, and fairness**, not just predictive power.  

This project reinforced that **data is only valuable if it can be communicated effectively**. Executives and stakeholders don’t just need predictions—they need **insights that drive actionable decisions**.  

---

## Skills & Tools Used  
- **Technical Tools:** Python, SQL, Scikit-Learn, Pandas, NumPy, Matplotlib  
- **Machine Learning Techniques:** PCA, Logistic Regression, Feature Scaling  
- **Evaluation Metrics:** Precision, Recall, F1-score, ROC-AUC  
- **Business Analytics:** Risk Analysis, Loan Repayment Prediction  

---
