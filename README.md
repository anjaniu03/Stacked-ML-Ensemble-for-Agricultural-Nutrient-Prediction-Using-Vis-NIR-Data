# Stacked-ML-Ensemble-for-Agricultural-Nutrient-Prediction-Using-Vis-NIR-Data

Developed by Team T14, MSc Data Science, University of Bristol

This project focuses on predicting soil and plant nutrient concentrations using Visible-Near Infrared (Vis-NIR) Spectral Data, developed as part of the MSc Data Science Mini Project at the University of Bristol (in collaboration with Dalhousie University). The goal was to design a stacked ensemble machine learning model capable of estimating multiple nutrient levels while reducing high spectral dimensionality and improving predictive accuracy across diverse agricultural datasets.

**Key Contributions**:
1. Data Cleaning & Imputation: Addressed missing nutrient values (e.g., Boron, Chloride, Aluminum) using XGBoost-based imputation and mean substitution, ensuring complete and reliable datasets.
2. Dimensionality Reduction: Applied Partial Least Squares (PLS) and feature binning (8nm window) to reduce over 4,200 spectral features to ~260, improving computational efficiency.
3. Model Development: Implemented Lasso Regression, Random Forest and XGBoost to predict nutrient concentrations, later combining them via a stacked ensemble framework for enhanced performance.

Evaluation Metrics: Used R² Score, RPD (Ratio of Performance to Deviation) and NRMSE to assess model performance across datasets.
Performance Highlights: Achieved up to 80% prediction accuracy for key nutrients, with a 25% improvement in RMSE following dimensionality optimization.

Methodology:
Data Preprocessing: Normalization, handling missing data, and dataset merging.
Feature Reduction: PCA evaluation followed by optimized PLS for meaningful spectral compression.
Model Training: Ensemble of regression algorithms with hyperparameter tuning using FLAML’s CASH framework.
Stacking & Validation: Integrated predictions of related nutrients (N, P, K) to improve generalization.

Results Summary:
XGBoost consistently outperformed other models on 5 out of 7 datasets.
Stacked ensemble approach improved predictive robustness across different seasons (Dry vs. Fresh).
Demonstrated feasibility of AI-driven soil nutrient prediction to support data-informed agricultural decisions.

Tech Stack:
Languages: Python
Libraries: Pandas, NumPy, Scikit-learn, XGBoost, FLAML, Matplotlib
Tools: Jupyter Notebook, Git, PowerPoint (presentation/reporting)

Future Work:
Explore heterogeneous stacking using deep learning base learners.
Experiment with autoencoder-based spectral feature extraction.
Incorporate environmental metadata (e.g., temperature, soil type) to enhance model generalization.

