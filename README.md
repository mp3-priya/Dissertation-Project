Machine Learning-Based Classification of BEVs and PHEVs

Project Overview:
This project focuses on classifying Battery Electric Vehicles (BEVs) and Plug-in Hybrid Electric Vehicles (PHEVs) using machine learning techniques. The study leverages real-world Washington State EV registration data to build accurate and interpretable classification models.
The goal is to support policy-making, infrastructure planning, and EV adoption analysis through data-driven insights.

Objectives:
Compare performance of ML models: SVM, GBM, and Hybrid Ensemble
Handle class imbalance using SMOTE
Improve prediction accuracy with feature engineering & preprocessing
Provide model interpretability using SHAP & LIME
Identify key factors influencing EV classification

Methodology
Dataset:
Source: Washington State EV Population Dataset
Records used: ~20,000 (due to hardware constraints)
Features include:
Vehicle type (BEV/PHEV)
Model year, make, electric range
MSRP and geographic attributes

Results:
SVM: 99% accuracy
GBM: 100% accuracy
Hybrid: 100% accuracy (best model)

Data Preprocessing:
Data cleaning & feature selection
One-hot encoding for categorical variables
Class imbalance handled using SMOTE
Train-test split (80/20, stratified)

Models Used:
Support Vector Machine (SVM)
Gradient Boosting Machine (GBM - XGBoost)
Hybrid Ensemble (SVM + GBM)


Hyperparameter Tuning:
GridSearchCV with cross-validation
Optimized using F1-score (macro)

Key Insights:
Electric Range is the strongest predictor
Model Year & Manufacturer significantly impact classification
SMOTE improved minority class (PHEV) detection drastically
Ensemble methods improved stability and generalisation

Tech Stack:
Python
Scikit-learn
XGBoost
Pandas, NumPy
Matplotlib, Seaborn
SHAP, LIME
Google Colab

How to Run:
# Clone the repository
git clone https://github.com/your-username/your-repo-name.git  

# Navigate to project folder
cd your-repo-name

# Install dependencies
pip install -r requirements.txt

# Run the notebook/script

Limitations:
Dataset reduced to 20,000 rows (hardware constraints)
Synthetic bias due to SMOTE
Limited geographic scope (Washington State only)

Future Work
Use full dataset for better generalisation
Include more socio-economic features
Deploy as a web-based prediction tool
Test deep learning models

Impact
This project contributes to:
Sustainable transportation research
EV infrastructure planning
Data-driven policymaking
