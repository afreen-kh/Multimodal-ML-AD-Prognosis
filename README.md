# An Improved Multi-Modal Based Machine Learning Approach for the Prognosis of Alzheimer’s Disease

**Afreen Khan, S. Zubair**  
*Journal of King Saud University – Computer and Information Sciences, 2020*

🔗 **Paper (PDF):** https://www.sciencedirect.com/science/article/pii/S1319157820303396 

---

## Overview

This repository documents the methodology, experimental pipeline, and key findings of the research paper:

The study proposes a **five-stage multi-modal machine learning pipeline** for early prognosis of Alzheimer’s Disease (AD), integrating MRI-derived biomarkers with cognitive assessment scores such as MMSE, CDR, and ASF.

The work emphasizes structured preprocessing, feature engineering, model validation, and performance evaluation, demonstrating that ensemble learning—particularly Random Forest, achieves superior diagnostic performance.

---

## Key Contributions

- Designed a **five-level sequential machine learning pipeline** for AD prognosis  
- Integrated **neuroimaging features (MRI)** with **clinical cognitive scores**
- Conducted extensive **exploratory data analysis (EDA)** and **feature selection**
- Evaluated **17 supervised ML classifiers**
- Demonstrated that **Random Forest with median imputation** yields the best performance
- Achieved **high diagnostic accuracy (≈87%)**, with strong sensitivity and specificity

---

## 📊 Dataset Description

- **Dataset Source:**  
  Open Access Series of Imaging Studies (OASIS)

- **Subjects:**  
  - 150 individuals  
  - 343 MRI sessions (Visit = 1 only)
  - Age range: 60–96 years

- **Modalities Used:**  
  - Structural MRI (T1-weighted, 1.5T scanner)
  - Neuropsychological and demographic features

### Key Features Utilized
- Age  
- Gender  
- Education (EDUC)  
- Socioeconomic Status (SES)  
- Mini-Mental State Examination (MMSE)  
- Clinical Dementia Rating (CDR)  
- Estimated Total Intracranial Volume (eTIV)  
- Normalized Whole Brain Volume (nWBV)  
- Atlas Scaling Factor (ASF)

> **Note:** Raw MRI data and subject-level clinical data are not included due to data access restrictions.

---

## Proposed Methodology

The study follows a **five-stage machine learning pipeline**:

<p align="center">
  <img src="figures/ml_multimodal_pipeline.png" alt="Multimodal ML Pipeline" width="700">
</p>

<p align="center">
  <em>Figure 1: Multimodal ML Pipeline</em> 
</p> 


### Data Preparation
- Missing value handling (median imputation)
- Outlier detection
- Feature scaling (standardization)
- Label encoding
- Exploratory data analysis (boxplots, KDEs, correlation heatmaps)

### Data Segregation
- Randomized splitting into:
  - Training set
  - Validation set
  - Test set

### Model Building
- Training of multiple ML classifiers
- Cross-validation (10-fold)
- Hyperparameter tuning (Grid Search)

### Model Prediction
- Performance evaluation on unseen test data
- Binary classification: Demented vs Non-Demented

### Performance Evaluation
- Accuracy
- Precision
- Recall (Sensitivity)
- Specificity
- F1-score
- ROC–AUC analysis
- Confusion matrix interpretation

---

## 🤖 Machine Learning Models Evaluated

A total of 17 supervised ML classifiers, including:

- Random Forest
- Extra Trees
- Gradient Boosting
- AdaBoost
- Decision Tree
- Logistic Regression (CV)
- Support Vector Machines (Linear & RBF)
- Naïve Bayes (Gaussian & Bernoulli)
- K-Nearest Neighbors
- Ridge Classifier
- SGD Classifier
- Multi-Layer Perceptron (MLP)

---

## Key Results

- **Best-performing model:** Random Forest  
- **Test Accuracy:** ~86.84%  
- **Sensitivity:** 80%  
- **Specificity:** 88%  
- **AUC:** ~0.87  

Random Forest demonstrated:
- Strong generalization
- Reduced overfitting
- Robust handling of multi-modal features

---

## Citation

If you use or reference this work, please cite:

```bibtex
@article{khan2020multimodal,
  title={An Improved Multi-Modal Based Machine Learning Approach for the Prognosis of Alzheimer’s Disease},
  author={Khan, Afreen and Zubair, Swaleha},
  journal={Journal of King Saud University -- Computer and Information Sciences},
  year={2020}
}
## 📁 Repository Structure

