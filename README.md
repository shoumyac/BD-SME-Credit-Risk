# When Machine Learning Fails: Establishing Boundary Conditions for Applied AI in SME Credit Risk Assessment

This repository contains the **data, code, and documentation** supporting the research paper submitted to *Applied Artificial Intelligence*. The project investigates the use of machine learning for predicting credit risk among **small and medium enterprises (SMEs)** in an emerging economy context (Bangladesh), with a strong emphasis on **responsible, interpretable, and reproducible applied AI**.

---

## Repository Contents

```
bd-sme-credit-risk/
│
├── data/
│   └── bangladesh_sme_final_with_split.csv
│
├── notebooks/
│   └── bd_sme_credit_pipeline_enhanced.ipynb
│
├── DATA_REPOSITORY_GUIDE.md
└── README.md
```

### File Descriptions

* **`bangladesh_sme_final_with_split.csv`**
  An anonymised SME-level dataset used in the study.
  It includes financial, operational, and categorical attributes collected for research purposes, along with a binary credit-risk outcome variable.

* **`bd_sme_credit_pipeline_enhanced.ipynb`**
  The complete Jupyter notebook implementing the modelling pipeline described in the paper, including:

  * data preprocessing and leakage prevention
  * tabular-only and tabular + TF-IDF models
  * stratified cross-validation
  * performance evaluation (ROC-AUC, PR-AUC, F1, Balanced Accuracy)
  * calibration analysis (Brier score, reliability curve)
  * SHAP-based explainability (global and local)

* **`DATA_REPOSITORY_GUIDE.md`**
  Documentation explaining the data and code deposition strategy, repository structure, and best practices for transparency and reproducibility.

---

## Research Context

Small and medium enterprises play a crucial role in emerging economies but often face limited access to formal credit due to information asymmetry and risk assessment challenges. This project evaluates **when and how applied machine learning can (and cannot) be used responsibly** for SME credit risk prediction under realistic data constraints.

Rather than maximising predictive accuracy, the study focuses on:

* leakage-safe evaluation
* honest cross-validation
* probability calibration
* explainability for decision support, not automation

---

## Data Ethics and Privacy

* All data are **fully anonymised**
* No personal identifiers (names, phone numbers, addresses) are included
* Data are used strictly for **academic research purposes**
* Values may be scaled or normalised for modelling and should not be interpreted as raw financial records

---

## Reproducibility

To reproduce the analysis:

1. Clone the repository
2. Open the notebook:

   ```
   notebooks/bd_sme_credit_pipeline_enhanced.ipynb
   ```
3. Run cells sequentially in a Python environment

### Environment (recommended)

* Python 3.9+
* pandas
* numpy
* scikit-learn
* xgboost
* shap
* matplotlib / seaborn

Exact package versions are documented inside the notebook.

---

## Notes on Results Interpretation

* Cross-validation results represent **out-of-sample performance**
* Models trained on the full dataset are used **only for diagnostic and explainability analysis**
* Figures such as SHAP plots and calibration curves are illustrative and not used to claim generalisation performance

---

## License

This repository is shared for **academic and non-commercial research use**.
Please cite the associated paper if you use this data or code.

---

## Contact

**Corresponding Author**
Shoumya Chowdhury
Faculty of Engineering and Information Technology
The University of Melbourne
Email: [shoumyac@student.unimelb.edu.au](mailto:shoumyac@student.unimelb.edu.au)

---

*This repository is provided to support transparency, reproducibility, and responsible use of applied artificial intelligence in financial decision-making.*
