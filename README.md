# HRV-Based Cardiac Risk Prediction System

## Overview

This project presents a data-driven approach for early cardiac risk prediction using Heart Rate Variability (HRV) signals combined with clinical data.

HRV is a non-invasive biomarker reflecting autonomic nervous system function, making it valuable for early detection of cardiovascular risk conditions such as cardiac autonomic neuropathy (CAN).

---

## Problem

Early detection of cardiac risk is challenging due to:

* High variability in physiological signals
* Noise and artifacts in ECG data
* Inter-patient variability
* Limited labeled medical datasets

Traditional approaches often struggle to generalize across real-world conditions.

---

## Data & Features

* Clinical data (demographics, labs, medical history)
* ECG-derived HRV features

Key HRV features:

* SDNN (standard deviation of RR intervals)
* RMSSD (short-term variability)
* Nonlinear features (entropy, SD1, SD2)

---

## System Approach

### Pipeline

* Clinical data preprocessing and merging
* ECG signal cleaning and R-peak detection
* HRV feature extraction
* Feature selection and scaling
* Model training and evaluation

---

### Models Evaluated

* Random Forest
* Logistic Regression
* XGBoost
* KNN
* SVM
* LightGBM
* AdaBoost

---

## Results & Observations

* XGBoost achieved the best performance after hyperparameter tuning
* HRV features provide strong predictive signals for cardiac risk

> Most performance improvements come from better feature extraction and preprocessing rather than model complexity.

This highlights that physiological signal modeling is primarily a **data representation and quality problem**.

---

## Visual Results

### Model Performance

<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/3d317e34-957d-484b-8bc9-d61a96083c3e" />

---

## Tech Stack

* Python
* Scikit-learn
* XGBoost, LightGBM
* NeuroKit2 (HRV analysis)
* Pandas, NumPy

---

## Repository Structure

```
├── notebook.ipynb
├── results/
├── README.md
└── requirements.txt
```

---

## Dataset

This project uses the CDED dataset from PhysioNet.

Due to size constraints, the dataset is not included.

👉 Download here:
https://physionet.org/content/cded/1.0.1/

---

## Research Context

HRV-based analysis is widely used in biomedical research for assessing cardiovascular and autonomic nervous system health.

Machine learning enables automated detection of subtle physiological patterns for early diagnosis.

---

## Future Work

* Deep learning on raw ECG signals
* Multi-modal health data integration
* Real-time monitoring systems

---

## Author

Raif Tanjim
