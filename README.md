# Dataset Balancing for Emission Classification Using Advanced Resampling Techniques

## Overview

This repository presents a comprehensive study on dataset balancing techniques for **emission classification (Low vs. High Emissions)**. The original dataset exhibited significant class imbalance, which can severely degrade machine learning model performance and bias predictions toward the majority class.

To mitigate this issue, multiple advanced resampling techniques were implemented, analyzed, and compared to produce a robust and fair dataset suitable for training reliable classification models.

---

## Original Dataset Statistics

| Metric | Value |
|--------|------|
| Total Samples | 400 |
| Class 0 — Low Emissions | 322 (80.50%) |
| Class 1 — High Emissions | 78 (19.50%) |
| Imbalance Ratio | 4.13 |

 The dataset showed a strong majority bias toward **Low Emissions**, making direct model training unreliable without balancing.

---

## Implemented Balancing Techniques

The following advanced resampling methods were applied and evaluated:

- SMOTE  
- ADASYN  
- Borderline-SMOTE  
- SMOTE + Tomek Links  

Each method was assessed based on:

- Class distribution balance  
- Duplicate and near-duplicate generation  
- Dataset cleanliness  
- Decision boundary quality  

---

## Balancing Results Comparison

| Technique | Total Samples | Class 0 | Class 1 | Imbalance Ratio | Exact Duplicates | Near Duplicates |
|----------|---------------|---------|---------|------------------|------------------|-----------------|
| SMOTE | 644 | 322 (50%) | 322 (50%) | 1.00 | 0% | 0% |
| ADASYN | 644 | 322 (50%) | 322 (50%) | 1.00 | 0% | 0% |
| Borderline-SMOTE | 644 | 322 (50%) | 322 (50%) | 1.00 | 0% | 0% |
| SMOTE + Tomek Links | 644 | 322 (50%) | 322 (50%) | 1.00 | 0% | 0% |

All techniques achieved perfect class balance without introducing duplicate samples.

---

## Recommended Technique

### SMOTE + Tomek Links

**Reasons for Recommendation:**

- Achieves perfect class balance (1:1 ratio)  
- Generates high-quality synthetic samples  
- Removes noisy and overlapping instances  
- Produces cleaner decision boundaries  
- Preserves dataset diversity  

This method provides the most reliable foundation for training robust emission classification models.

---

## Repository Contents

---

## Research Significance

Balanced datasets significantly improve:

- Classification accuracy  
- Minority class recall  
- F1-score stability  
- Model generalization capability  
- Fairness in predictions  

This preprocessing pipeline ensures robustness and reliability in emission prediction systems.

---

## Authors

**Dr. Shahul Hameed Chettali**  
Assistant Professor, Department of CSE (Cyber Security)  
Vel Tech Rangarajan Dr. Sagunthala R&D Institute of Science and Technology  
Chennai, Tamil Nadu, India  
drshahulcse@gmail.com  

**S. Alfiya**  
Assistant Professor, Department of Computer Science and Engineering  
Vel Tech Multi Tech Dr. Rangarajan Dr. Sakunthala Engineering College  
Chennai, Tamil Nadu, India  
alfiya118@gmail.com  

---

## Author Contributions

### Dr. Shahul Hameed Chettali 

- Research conceptualization  
- Methodology design and validation  
- Implementation of balancing algorithms  
- Statistical evaluation and analysis  
- Result interpretation  
- Manuscript drafting and technical review  
- Supervision  

### S. Alfiya 

- Dataset preprocessing  
- Experimental execution  
- Result compilation  
- Literature review support  
- Visualization and formatting  

---



Balanced datasets and analysis outputs:

