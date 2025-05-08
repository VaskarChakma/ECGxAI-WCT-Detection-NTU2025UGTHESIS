# 🫀 ECG-based Wide QRS Complex Tachycardia (WCT) Detection Using Ensemble Machine Learning Models

This repository contains the code, data, and results for my undergraduate thesis:  
**"Using the ECGxAI Model for the Diagnosis of Wide QRS Complex Tachycardia (WCT)"**.  
The project focuses on developing an explainable AI system to detect WCT from ECG signals using ensemble learning techniques, evaluated using 10-fold cross-validation.

---

## ⚙️ Key Features

- **📦 Dataset**  
  Utilizes the [MIMIC-IV-ECG](https://physionet.org/content/mimic-iv-ecg/1.0/) dataset, cleaned and preprocessed for machine learning tasks.

- **📊 Machine Learning Models**  
  Ensemble models used for detection:
  - CardioForest (custom RandomForest)
  - XGBoost
  - LightGBM
  - Gradient Boosting

- **🔁 Evaluation Technique**  
  - 10-fold Cross-Validation  
  - Data split ratio: 10:9 (Train:Test)

- **⚖️ Imbalanced Data Handling**  
  - SMOTE for minority class oversampling

- **🧼 Data Preprocessing**:
  - Median imputation for missing values  
  - Standardization  
  - Noise injection  
  - Label encoding  
  - Feature type optimization

- **📈 Performance Metrics**
  - Accuracy
  - Balanced Accuracy
  - Precision
  - Recall
  - F1 Score
  - ROC AUC

---

## 🖼️ Framework Overview

![Model Framework](path/to/your_framework_image.png)  
*Replace the path above with your actual image filename.*

---

## 📊 Results Summary

| Model            | Accuracy (Test) | Balanced Accuracy (Test) | Precision (Test) | Recall (Test) | F1 Score (Test) | ROC AUC (Test) |
|------------------|------------------|----------------------------|-------------------|----------------|------------------|----------------|
| **CardioForest**     | 0.9495           | 0.8832                     | 0.9489            | 0.7762         | 0.8538           | 0.8833         |
| **XGBoost**          | 0.8835           | 0.7168                     | 0.8810            | 0.4479         | 0.5937           | 0.8495         |
| **LightGBM**         | 0.8422           | 0.6435                     | 0.6787            | 0.3229         | 0.4374           | 0.7806         |
| **Gradient Boosting**| 0.9179           | 0.8006                     | 0.9282            | 0.6113         | 0.7214           | 0.8544         |

> 📌 *Each model was evaluated with 10-fold cross-validation using a 10:9 train-test split.*

---

## 📖 Dataset Details

- **Source**: [MIMIC-IV-ECG on PhysioNet](https://physionet.org/content/mimic-iv-ecg/1.0/)
- **Size**: 800,000+ ECG records from 160,000+ patients
- **Target Variable**: Binary classification of WCT (`wct_label_encoded`)
- **Key Features Used**:
  - `rr_interval`, `qrs_duration`, `p_onset`, `qrs_end`, `t_axis`, `qrs_axis`, etc.

---

## 🧠 Author

**[Vaskar Chakma](https://scholar.google.com/citations?user=aE4O5HUAAAAJ&hl=en)**  
Undergraduate Student, School of Artificial Intelligence & Computer Science  
Nantong University, China

---

## 🎓 Thesis Supervisor

**[Dr. Gao Zhan](https://ai.ntu.edu.cn/2024/0817/c9718a246517/page.htm)**  
Professor, School of Artificial Intelligence & Computer Science  
Nantong University, China

---
