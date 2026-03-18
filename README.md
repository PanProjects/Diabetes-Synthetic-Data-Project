# Diabetes Synthetic Data Generation  
## Bio-data Analysis

---

## 📌 Overview

This project explores the use of **synthetic medical data generation** techniques to improve machine learning performance on imbalanced healthcare datasets. The focus is on diabetes prediction using the **BRFSS 2015 Diabetes Health Indicators dataset**.

---

## 👥 Team Members

- **Member 1:** Panteleimon Naoum  
- **Member 2:** Andreas Gkanas  
- **Member 3:** Kerkyra Dimitisianou  

---

## 🧭 Research Axis

**Synthetic Medical Data Generation: Opportunities and Challenges for GenAI-Based Augmentation (Axis 5)**

---

## 📊 Dataset

- **Name:** Diabetes Health Indicators Dataset  
- **Source:** BRFSS 2015 (Behavioral Risk Factor Surveillance System)  
- **File Used:** `diabetes_012_health_indicators_BRFSS2015.csv`  
- **Classes:**
  - 0 → No diabetes  
  - 1 → Prediabetes (minority class)  
  - 2 → Diabetes  

---

## 🎯 Motivation

Diabetes is one of the most widespread chronic diseases globally. Real-world medical datasets often suffer from **class imbalance**, making it difficult to train reliable predictive models—especially for minority classes such as prediabetes.

Synthetic data generation offers a promising solution by:
- Balancing class distributions  
- Enhancing model generalization  
- Preserving data privacy  

---

## ❓ Research Questions

1. **Can synthetic data generation techniques (CTGAN, VAE, SMOTE) improve classifier performance on imbalanced medical datasets?**

2. **Which method best preserves the statistical properties and feature relationships of the original dataset?**

3. **How does data augmentation affect prediction performance for the minority class (prediabetes)?**

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Handling missing values  
- Feature normalization  
- Exploratory Data Analysis (EDA)  

---

### 2. Synthetic Data Generation Techniques

- **SMOTE** (Synthetic Minority Over-sampling Technique)  
- **CTGAN** (Conditional GAN for tabular data, via SDV library)  
- **Variational Autoencoder (VAE)** implemented in PyTorch  

---

### 3. Model Training

The following classifiers will be trained **before and after augmentation**:

- Random Forest  
- XGBoost  

---

### 4. Evaluation Metrics

- **F1-score (macro)**  
- **AUC-ROC**  
- **Precision & Recall per class**  

---

### 5. Synthetic Data Quality Assessment

- **Kolmogorov–Smirnov (KS) Test** for distribution comparison  
- **t-SNE visualizations** for feature space similarity  

---

## 📈 Expected Outcomes

- Improved classification performance, especially for **prediabetes (class 1)**  
- Deep generative models (**CTGAN, VAE**) expected to outperform SMOTE in:
  - Preserving statistical distributions  
  - Maintaining feature correlations  
- A **comparative analysis** of all methods with practical recommendations  

---

## 📚 References

1. Chawla, N. V., Bowyer, K. W., Hall, L. O., & Kegelmeyer, W. P.  
   *SMOTE: Synthetic Minority Over-sampling Technique*  
   Journal of Artificial Intelligence Research, 2002  

2. Xu, L., Skoularidou, M., Cuesta-Infante, A., & Veeramachaneni, K.  
   *Modeling Tabular Data using Conditional GAN*  
   NeurIPS, 2019  

3. Xie, Z., Nikolov, O., Wascher, G., & Watkins, E.  
   *Building Risk Prediction Models for Type 2 Diabetes Using Machine Learning Techniques*  
   Preventing Chronic Disease, 2019  

4. Kingma, D. P., & Welling, M.  
   *Auto-Encoding Variational Bayes*  
   ICLR, 2014  

5. Zhao, J., et al.  
   *Generative AI for Medical Data Augmentation*  
   IEEE Reviews in Biomedical Engineering, 2024  

---

## 🚀 Future Work

- Hyperparameter tuning of generative models  
- Evaluation on additional medical datasets  
- Integration with privacy-preserving techniques (e.g., differential privacy)  
- Deployment in real-world clinical decision support systems  

---

## 🛠️ Technologies & Tools

- Python  
- Scikit-learn  
- XGBoost  
- PyTorch  
- SDV (Synthetic Data Vault)  
- Pandas, NumPy  
- Matplotlib / Seaborn  

---

## 📬 Contact

For questions or collaboration, feel free to reach out to the team members.

---