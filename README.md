# Breast Cancer Prediction Project

This project analyzes a breast cancer dataset (`dataR2.csv`) using Python and machine learning in a Jupyter Notebook (`breast-cancer.ipynb`).


## Project Overview
This project explores several machine learning models to classify patients as healthy or not healthy based on biomedical features.  
The models tested include:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- Support Vector Machine (SVM, RBF kernel)

The goal was to identify the model that achieves the best balance of **accuracy, precision, recall, F1-score, and ROC AUC**, with a particular focus on recall (minimizing false negatives is critical in a medical context).

---

## Project Structure
```markdown
notebooks/
│── 01_EDA.ipynb
│── 02_Logistic_Regression.ipynb
│── 03_Ridge.ipynb
│── 04_Tree_Based.ipynb
│── 05_SVM.ipynb
│── 06_Model_Comparison.ipynb
data/
│── dataR2.csv
```

---

## Key Results

| Model                  | Best Threshold | Accuracy | Precision | Recall | F1-score | ROC AUC |
|-------------------------|----------------|----------|-----------|--------|----------|---------|
| Logistic Regression     | 0.3            | 0.75     | 0.71      | 0.92   | 0.80     | 0.804   |
| Decision Tree           | 0.4–0.3        | 0.88     | 0.81      | 1.00   | 0.90     | 0.671   |
| Random Forest           | 0.3            | 0.79     | 0.72      | 1.00   | 0.84     | 0.839   |
| Gradient Boosting       | 0.3            | 0.92     | 0.87      | 1.00   | 0.93     | 0.888   |
| SVM (RBF)               | 0.4            | 0.88     | 0.86      | 0.92   | 0.89     | 0.874   |

**Best Model:** Gradient Boosting Classifier, which achieved the strongest overall performance (Accuracy 0.92, Recall 1.0, F1-score 0.93).


--- 
## Installation

To reproduce the experiments, create the Conda environment from the `environment.yml` file:

```bash
conda env create -f environment.yml
conda activate cleanpy
```
---
## Main libraries used:
- Python 3.x
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn



