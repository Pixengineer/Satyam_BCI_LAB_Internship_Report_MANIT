# Satyam_BCI_LAB_Internship_Report_MANIT

An advanced Brain-Computer Interface (BCI) computational framework designed for the automated, early-stage screening of clinical depression using multi-channel Electroencephalography (EEG) signals. Developed during the research internship at the BCI Laboratory, Department of Computer Science and Engineering, Maulana Azad National Institute of Technology (MANIT), Bhopal.

## 🧠 Core Engineering Framework
* **Dataset Utilization:** Processes the comprehensive MODMA dataset comprising continuous resting-state bio-signals.
* **Channel Topography:** Optimized for a minimal, consumer-grade frontalis scalp array covering **Fp1, Fp2, and Fz** channels.
* **Signal Preprocessing:** Implements MNE-Python routines for artifact rejection ($>500\mu V$) and 5th-order digital Butterworth filtering (0.5–40 Hz).
* **Feature Engineering:** Extracts Power Spectral Density (PSD) markers and computes Frontal Alpha Asymmetry (FAA) indices.
* **Classification Pipeline:** * Evaluates optimized ensemble models (**Random Forest / XGBoost**) utilizing a locked-seed **SMOTE** neighborhood density inflation engine to achieve a baseline validation accuracy of **85.71%** with **100% precision** for the target MDD class.
  * Explores end-to-end **1D-CNN** architectures utilizing spatial-temporal convolutions and batch normalization to bridge the cross-subject generalization gap under Leave-One-Subject-Out (LOSO) cross-validation.****
