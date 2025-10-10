# Stacked-ML-Ensemble-for-Agricultural-Nutrient-Prediction-Using-Vis-NIR-Data

**The Team**: Anjani Upadhyay, Hangwei Pu, Sahana Somani, Shaoshuai Li

**Degree**: MSc Data Science, University of Bristol (2024–2025)

**Supervisor**: Felipe Campelo

Agriculture increasingly depends on data, but laboratory soil testing is slow and expensive. This project focuses on predicting soil and plant nutrient concentrations using Visible-Near Infrared (Vis-NIR) Spectral Data, developed as part of the MSc Data Science Mini Project at the University of Bristol (in collaboration with Dalhousie University). Our group decided to design a stacked ensemble machine learning model capable of estimating multiple nutrient levels while tackling the challenges of noisy, high dimensional and incomplete data and improving predictive accuracy across diverse seasonal agricultural datasets.

### Key Questions:
1. How can we extract meaningful insights from 4,200+ spectral features per sample?
2. Can machine learning be used to replace or at least support traditional laboratory nutrient testing?
3. What modelling strategies can improve accuracy when datasets have missing or inconsistent values?
4. Is it possible to build a stacking pipeline to predict multiple nutrients from fresh/dried modes at once?

### Supporting Technologies:
* **Core Programming & Data Analysis (Python)** - Pandas, NumPy, Matplotlib, Seaborn
* **Machine Learning & AutoML** - Scikit-learn, XGBoost, LightGBM, FLAML
* **Development & Collaboration** - Jupyter Notebooks, Google Colaboratory, LaTeX (via Overleaf), GitHub, PowerPoint

**Methodology**:

1. **Data Preprocessing**: Cleaned and merged multiple “Fresh” and “Dry” season datasets, addressed missing nutrient values (e.g. Boron, Chloride, Aluminum) using XGBoost based imputation and mean substitution, ensuring complete and reliable datasets.
2. **Dimensionality Reduction**: Reduced 4,200 spectral features to 263 using feature binning (8nm window) and Partial Least Squares (PLS) improving interpretability and reducing noise.
3. **Model Training**: Trained and compared Lasso, ElasticNet, Random Forest and XGBoost models, tuning hyperparameters automatically using FLAML’s CASH optimisation framework.
4. **Stacked Ensemble**: Combined the best performing models into a stacked regression ensemble to integrated predictions of related nutrients, boosting generalisation and minimising R² Score, RPD and NRMSE.

**Results & Insights**:

* Achieved up to 80% accuracy for key nutrient predictions (e.g. Nitrogen, Phosphorus, Potassium).
* RMSE improved by 25% after dimensionality reduction and imputation optimisation.
* XGBoost consistently outperformed other algorithms across 5 of 7 datasets, but ensemble learning offered greater robustness across seasons (Dry vs. Fresh).
* Demonstrated feasibility of using machine learning in soil nutrient prediction to support data-informed agricultural decisions.

Working with real agricultural data showed how much of data science lies in cleaning, transforming and validating messy inputs. The biggest takeaway? Even small improvements in model accuracy can translate into real world value for farmers, enabling faster and more sustainable soil monitoring.
