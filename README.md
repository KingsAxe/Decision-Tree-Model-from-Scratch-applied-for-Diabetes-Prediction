## Diabetes Risk Prediction — Decision Tree (From Scratch)

This project implements a **Decision Tree Classifier** completely **from scratch** in Python to predict diabetes risk based on clinical and lifestyle features.  
The focus was on **understanding the internals** of tree-based learning, **evaluating performance manually**, and **building interpretability tools** (like SHAP) without external ML libraries.



## Features

- **Custom Decision Tree Implementation** — built using pure Python and NumPy.  
- **Manual Training Pipeline** — includes a self-coded training routine (`My_train`) and prediction flow.  
- **Cross-Validation System** — evaluates model robustness without relying on sklearn utilities.  
- **Handcrafted SHAP Approximation** — feature importance estimated via permutation accuracy drop.  
- **Metric Suite (from scratch)** — accuracy, precision, recall, and F1-score computed manually.  
- **Reproducible Notebook** — demonstrates the workflow, dataset preprocessing, and model evaluation.



## Dataset
The model was trained on a **Diabetes dataset** containing clinical and demographic indicators such as:
- Polyuria  
- Polydipsia  
- Sudden weight loss  
- Partial paresis  
- Obesity  
- Gender and other health symptoms  

All features were label-encoded to prepare for numerical computation.


## Insights
Using the approximate SHAP feature importance method, the most influential factors were found to be:
- **Polyuria**
- **Partial Paresis**
- **Polydipsia**
- **Gender**
- **Alopecia**

These align with known medical correlations for diabetes diagnosis.


## Future Work
- Extend to a **Random Forest or Gradient Boosting** ensemble.  
- Add **per-instance SHAP visualization**.  
- Integrate **streamlit-based UI** for real-time predictions.  
- Benchmark against **scikit-learn DecisionTreeClassifier** for comparison.


## Requirements
- Python 3.8+
- NumPy  
- Matplotlib
