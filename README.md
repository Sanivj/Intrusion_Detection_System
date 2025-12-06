# 💻 WOA-F2I Optimized Intrusion Detection System for High-Accuracy Network Security

This project presents a novel, lightweight, and highly accurate **Intrusion Detection System (IDS)** specifically designed for **Software-Defined Networking (SDN)** environments[cite: 108, 121, 449]. The key innovation is the **WOA-F2I** framework, a hybrid feature-selection approach that addresses the challenge of high-dimensional traffic data in modern networks[cite: 84, 309, 248].

---

## 🌟 Key Features and Contributions

- **Hybrid Feature Selection (WOA-F2I):** Integrates statistical ranking methods (**Fisher Score** and **Information Gain**) with the **Whale Optimization Algorithm (WOA)** meta-heuristic to automatically determine the most informative and minimal subset of features[84, 88, 309, 248].

- **Dimensionality Reduction:** Reduces the feature space of the UNSW-NB-15 dataset by approximately **44%** (from 48 features to 27)[441, 460].

- **High Performance:** Achieves superior detection metrics compared to full-feature and traditional approaches, with the **Random Forest** classifier reaching an accuracy of **99.26%**, precision of **0.99**, and recall of **0.98** on the optimized subset[421, 434, 431, 433].

- **Computational Efficiency:** Reduces model training time from approximately 1400 seconds to **325 seconds**, making the resulting IDS model suitable for real-time deployment on resource-constrained SDN controllers[423, 135].

- **Robust Security:** Focuses on safeguarding the centralized SDN controller against various attacks (DoS/DDoS, Spoofing, Man-in-the-Middle)[131, 167].

---

## 🛠️ Methodology Overview

The WOA-F2I framework is a systematic pipeline designed for efficiency and accuracy[312].

1. **Data Preparation:** Includes preprocessing steps such as cleaning, encoding, and normalization of the UNSW-NB-15 SDN traffic dataset[320, 364].

2. **Feature Ranking:** Features are pre-ranked using **Fisher Score** and **Information Gain** to evaluate discriminative power[262, 365].

3. **Optimal Subset Search:** The **Whale Optimization Algorithm (WOA)** searches for an optimal number of features (*k*) by minimizing a fitness function balancing accuracy and subset compactness[279, 343, 345].

4. **Model Training:** Machine learning classifiers including **Random Forest**, **KNN**, **Logistic Regression**, and **SVM** are trained on the selected optimal features[355, 372].

5. **Evaluation:** Performance is validated using Accuracy, Precision, Recall, and F1-Score metrics[358, 373].

---

## 💾 Dataset

The project utilizes the **UNSW-NB-15 dataset**, which contains flow-level SDN traffic, including normal and attack instances[316, 390, 391].

**Dataset Link:**  
https://drive.google.com/file/d/15PqnOm13BYiUvDLnybik5_ZKjOKAa6CA/view?usp=drivesdk

---

## 🚀 Results Summary (Random Forest Classifier)

The model trained on the WOA-F2I optimized subset (27 features) yielded the following performance metrics:

| Metric          | Optimized Subset (WOA-F2I) |
|-----------------|----------------------------|
| **Accuracy**     | **99.26%**      |
| **Precision**    | **0.99**        |
| **Recall**       | **0.98**        |
| **F1-Score**     | **0.99**        |
| **Training Time**| **325 seconds** |

--- 
