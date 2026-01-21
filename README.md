# Astrophysical-Object-Classification
Star Classification using Random Forest (SDSS Dataset)
This repository contains a machine learning project that performs astronomical object classification using a Random Forest Classifier. The goal is to classify celestial objects into GALAXY, STAR, and QSO (Quasar) classes using photometric and spectroscopic features from the Sloan Digital Sky Survey (SDSS) dataset.

The implementation includes data exploration, preprocessing, model training, evaluation, feature importance analysis, and cross-validation, all demonstrated in a Jupyter Notebook

🎯 Project Objectives

Perform multi-class classification of astronomical objects

Apply Random Forest for robust, non-linear decision boundaries

Analyze feature importance to understand astrophysical relevance

Evaluate model performance using standard ML metrics

📊 Dataset Description

Source: Sloan Digital Sky Survey (SDSS)

Total Samples: 100,000

Target Classes:

GALAXY

STAR

QSO

🔢 Key Features Used

Photometric bands: u, g, r, i, z

Positional data: alpha, delta

Spectroscopic & observational data:

redshift

plate

MJD

fiber_ID

spec_obj_ID

run_ID, rerun_ID, cam_col, field_ID

No missing values were found in the dataset after inspection 

vertopal.com_TRW_RandomForest (…

.

🔍 Exploratory Data Analysis (EDA)

Dataset type and memory usage inspection

Statistical summary using describe()

Class distribution visualization

GALAXY is the majority class

STAR and QSO are minority classes

EDA helps verify class imbalance and feature ranges before training.

🧹 Data Preprocessing

Forward-fill strategy used for safety (ffill)

Feature selection performed manually based on relevance

Target variable: class

Stratified train–test split:

80% Training

20% Testing

🤖 Model Used
Random Forest Classifier

n_estimators = 100

random_state = 42

Handles high-dimensional and non-linear data efficiently

Suitable for tabular astronomical datasets

📈 Model Evaluation
✅ Performance Metrics

Accuracy: 98%

Precision / Recall / F1-score: High across all classes

Confusion Matrix: Visualized using heatmap

🔁 Cross-Validation

5-Fold Cross Validation

Mean CV Score: ~97.88%

This confirms the model’s stability and robustness across different data splits.

🧠 Feature Importance Analysis

Top contributing features include:

redshift (most dominant)

z, g, u photometric bands

spec_obj_ID, plate, r

Feature importance visualization helps interpret which astrophysical attributes most influence classification decisions.

🛠️ Technologies Used

Language: Python

Libraries:

Pandas

NumPy

Scikit-learn

Matplotlib

Seaborn

Environment: Jupyter Notebook

🚀 Applications

Astronomical object classification

Astrophysics data analysis

Large-scale survey automation

Scientific data-driven discovery

📌 Future Improvements

Try Gradient Boosting / XGBoost

Handle class imbalance with SMOTE

Add Explainable AI (SHAP / LIME)

Deploy as a web app (Flask / Streamlit)


This project is intended for educational and academic use.
Feel free to use and modify with proper attribution.
