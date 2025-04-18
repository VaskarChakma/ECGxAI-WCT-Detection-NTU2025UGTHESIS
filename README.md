# 🫀 ECG-based Wide QRS Complex Tachycardia (WCT) Detection Using Ensemble Machine Learning Models

This repository contains the code, data, and results for my undergraduate thesis:  
**"Using the ECGxAI Model for the Diagnosis of Wide QRS Complex Tachycardia (WCT)"**.  
The project focuses on developing an explainable AI system to detect WCT from ECG signals using ensemble learning techniques like XGBoost, LightGBM, Random Forest, and Gradient Boosting, evaluated through Monte Carlo simulations.

---

## ⚙️ Key Features

- **📦 Dataset**:  
  Uses a cleaned version of the [MIMIC-IV-ECG](https://physionet.org/content/mimic-iv-ecg/1.0/) dataset.

- **📊 Machine Learning**:  
  Implements multiple ensemble models:  
  - XGBoost  
  - LightGBM  
  - Random Forest  
  - Gradient Boosting  

- **🔁 Monte Carlo Evaluation**:  
  Repeats training/testing across 10 randomized simulations for robust metrics.

- **⚖️ Imbalanced Data Handling**:  
  Uses SMOTE to address class imbalance during training.

- **🧼 Data Preprocessing**:
  - NaN imputation using median values  
  - Noise injection for augmentation  
  - Standardization  
  - Label encoding  
  - Feature type handling

- **📈 Performance Metrics**:
  - Accuracy  
  - F1 Score  
  - R² Score (for probabilistic output)

- **🖼️ Visualization**:
  - Boxplots for comparing model metrics across Monte Carlo runs  
  - Auto-saves plots for Accuracy, F1 Score, and R² Score

---


---

## 📊 Results (Monte Carlo Simulation)

| Model            | Avg Accuracy | Avg F1 Score | Avg R² Score |
|------------------|--------------|--------------|---------------|
| XGBoost          | ~0.6656      | ~0.6454      | ~0.9995       |
| LightGBM         | ~0.6532      | ~0.6396      | ~0.9998       |
| RandomForest     | ~0.6946      | ~0.6589      | ~0.9996       |
| GradientBoosting | ~0.6368      | ~0.6280      | ~0.9999       |

> 📌 *Note: These values are averaged over 10 simulations with 10% test splits each time.*

---

## 📖 Dataset Details

- **Source**: [MIMIC-IV-ECG on PhysioNet](https://physionet.org/content/mimic-iv-ecg/1.0/)
- **Size**: 800,000+ ECG records from 160,000+ patients
- **Target Variable**: WCT classification (`wct_label_encoded`)
- **Key Features Used**:
  - `rr_interval`, `qrs_duration`, `p_onset`, `qrs_end`, `t_axis`, `qrs_axis`, and more...

---




## 🧠 Author

**[Vaskar Chakma](https://scholar.google.com/citations?user=aE4O5HUAAAAJ&hl=en)**  
Undergraduate Degree Student, School of Artificial Intelligence & Computer Science  
Nantong University, China

---
## 🧠 Thesis Supervisor

**[Dr. Gao Zhan](https://ai.ntu.edu.cn/2024/0817/c9718a246517/page.htm)**  
Professor, School of Artificial Intelligence & Computer Science  
Nantong University, China

---
