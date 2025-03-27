# ECG-based Wide QRS Complex Tachycardia (WCT) Detection Using Ensemble Machine Learning Models

This repository contains the code, data, and resources for my undergraduate thesis: **"Using the ECGxAI Model for the Diagnosis of Wide QRS Complex Tachycardia (WCT)"**. The project focuses on developing an explainable AI system to detect WCT from ECG signals using ensemble machine learning models (XGBoost, LightGBM, Random Forest, Gradient Boosting).

## 📋 Key Features
- **Dataset**: Uses the [MIMIC-IV-ECG](https://physionet.org/content/mimic-iv-ecg/1.0/) dataset with 800,000+ ECG recordings
- **Models**: Implements ensemble models (XGBoost, LightGBM, etc.) for high-accuracy WCT detection
- **Explainability**: Integrates SHAP, LIME, and feature importance analysis for model transparency
- **Performance**: Achieves near-perfect accuracy (99.98%) and ROC AUC (1.0) in simulations
- **Preprocessing**: Includes robust data cleaning, outlier handling, and PCA for dimensionality reduction



## 📊 Results
| Model            | Accuracy | F1 Score | ROC AUC | RMSE   |
|------------------|----------|----------|---------|--------|
| XGBoost          | 0.9998   | 0.9998   | 0.9999  | 0.0071 |
| LightGBM         | 0.9997   | 0.9996   | 0.9998  | 0.0122 |
| RandomForest     | 0.9995   | 0.9994   | 0.9996  | 0.0122 |
| GradientBoosting | 0.9993   | 0.9992   | 0.9995  | 0.0158 |


## 📖 Dataset Details
- **Source**: [MIMIC-IV-ECG on PhysioNet]([https://physionet.org/content/mimic-iv-ecg/1.0/](https://physionet.org/content/mimic-iv-ecg/1.0/))
- **Size**: 800,000+ ECGs from 160,000 patients
- **Features**: RR interval, QRS duration, P/T-wave metrics, filtering parameters,......
- **Preprocessing**: Median imputation, outlier removal, PCA

## 📜 References
1. MIMIC-IV-ECG: Diagnostic Electrocardiogram Matched Subset: Gow, B., Pollard, T., Nathanson, L. A., Johnson, A., Moody, B., Fernandes, C., Greenbaum, N., Waks, J. W., Eslami, P., Carbonati, T., Chaudhari, A., Herbst, E., Moukheiber, D., Berkowitz, S., Mark, R., & Horng, S. (2023). MIMIC-IV-ECG: Diagnostic Electrocardiogram Matched Subset (version 1.0). PhysioNet. https://doi.org/10.13026/4nqg-sb35.


## 🙏 Acknowledgments
- Supervisor: Dr. Gao Zhan, Professor, School of Artificial Intelligence and Computer Science, Nantong University




