# AI-ML
# XAI-FUSION: Hybrid Explainable AI for IoT/IIoT Intrusion Detection

## Overview

*XAI-FUSION* is a hybrid explainable artificial intelligence (XAI) framework designed to enhance the transparency, accuracy, and trustworthiness of intrusion detection systems (IDS) in modern IoT/IIoT networks. This project leverages the DNN-EdgeIIoT dataset and integrates SHAP, LIME, and LEMNA explanation methods to provide both global and local interpretability for network security analytics.

---

## Features

- *Hybrid XAI Fusion:* Weighted combination of SHAP, LIME, and LEMNA for comprehensive, robust explanations.
- *High Detection Accuracy:* XGBoost-based classifier achieves an F1-score of 0.91 on the DNN-EdgeIIoT dataset.
- *Privacy-Preserving Explanations:* Differential privacy (Laplace noise) and feature masking to protect sensitive network data.
- *Edge-Ready:* Optimized for real-time analysis and resource-constrained deployment (e.g., Raspberry Pi).
- *Rich Visual Analytics:* Includes confusion matrix, t-SNE projection, ROC curve, and comparative performance plots.
- *Progress Monitoring:* Uses progress bars to track explanation generation on large datasets.

---

## Dataset

- *DNN-EdgeIIoT:* Realistic IoT/IIoT network traffic dataset with 646,149 samples and 14 attack types.
- *Features Used:* Network-layer and protocol-specific features (e.g., frame.time, ip.src_host, arp.opcode, icmp.checksum).

---

## Results (from code and notebook)

- *Confusion Matrix:*  
  ![Confusion Matrix](Screenshot-984.jpg)
- *t-SNE Projection:*  
  ![t-SNE](Screenshot-987.jpg)
- *Comparative Metrics:*  
  ![Comparative Table](Screenshot-983.jpg)
- *ROC Curve:*  
  ![ROC Curve](Screenshot-985.jpg)

- *Classification Report:*

- precision recall f1-score support
0 1.00 0.83 0.90 323129
1 0.85 1.00 0.92 323020
accuracy 0.91 646149
macro avg 0.93 0.91 0.91 646149
weighted avg 0.93 0.91 0.91 646149


- *Performance Highlights:*
- *F1-Score:* 0.91 (proposed) vs. 0.79 (baseline)
- *Explanation Latency:* 1.45s/alert (proposed) vs. 2.78s (baseline)
- *Adversarial Robustness:* 75% (proposed) vs. 60% (baseline)
- *Explanation Consistency:* 79% (proposed) vs. 61% (baseline)
- **t-SNE and confusion matrix visualizations confirm effective separation and detection of attack traffic.

---

## How to Run

1. Clone this repository.
2. Install requirements:
3. 3. Place the DNN-EdgeIIoT dataset CSV in the working directory.
4. Run the main notebook or Python scripts to preprocess, train, and evaluate the model.
5. View results in the notebook or output folder.

---
