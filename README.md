# DLBS-VEHMS: A Dual-Layer based Blockchain-Secured Framework for Trustworthy Vehicular Engine Health Monitoring System and Fault Diagnosis

## Overview
This repository contains the implementation of **DLBS-VEHMS**, an intelligent and secure framework capable of predicting engine failures from imbalanced sensor data. The system introduces a **"Verify-then-Predict"** protocol that guarantees data provenance and ensures reliable, secure decision-making at the edge.

**Authors:** Md. Shahidul Islam Prodhan & Meheraj Hossain
**Institution:** Green University of Bangladesh (Department of Computer Science and Engineering)

## Key Contributions
1. **Dual-Stage Machine Learning Pipeline:** - **Stage 1 (Detection):** A 1D-Convolutional Neural Network (1D-CNN) accurately identifies machine failures from raw sensor data.
   - **Stage 2 (Diagnosis):** An XGBoost classifier activates to provide granular multi-class fault diagnosis.
2. **Data Imbalance Handling:** Utilizes SMOTE to synthetically balance rare failure events within the training set.
3. **VehiChain Security Layer:** A lightweight, blockchain-based integrity layer utilizing SHA-256 cryptographic hashing to detect tampering at the Electronic Control Unit (ECU).

## Dataset
Trained and evaluated on the **AI4I 2020 Predictive Maintenance Dataset** (10,000 data points, 14 features).

## Results & Performance
* **Detection Performance:** The 1D-CNN pipeline achieved an ROC-AUC of **0.977** and a Recall of **0.85**.
* **Security Feasibility:** The VehiChain layer demonstrated a **100% tamper detection rate** with a negligible processing latency of **0.0053 ms**.

## Citation
> Md. Shahidul Islam Prodhan, Meheraj Hossain. (2026). *DLBS-VEHMS: A Dual-Layer based Blockchain-Secured Framework for Trustworthy Vehicular Engine Health Monitoring System and Fault Diagnosis*. Capstone Thesis, Green University of Bangladesh.

## License
[MIT License](LICENSE)
