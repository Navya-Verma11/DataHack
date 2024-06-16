# DataHack 2024 - COVID-19 Vaccine Prediction Project

## Problem Statement
During the COVID-19 pandemic, understanding public willingness to take vaccines is crucial for effective vaccination campaigns. This project aims to predict vaccine uptake using demographic, behavioral, and attitudinal survey data.

## Approach
1. **Data Exploration and Preprocessing:**
   - Explored the provided datasets (`training_set_features.csv`, `training_set_labels.csv`, `test_set_features.csv`) to understand missing values, data types, and distributions.
   - Imputed missing values using appropriate strategies (median for numerical features, mode for categorical features).
   - Performed exploratory data analysis (EDA) to visualize distributions, correlations, and insights into the data.

2. **Feature Engineering:**
   - Created pipelines for preprocessing data, including handling categorical variables (using one-hot encoding) and scaling numerical features (using standardization).

3. **Modeling:**
   - Evaluated multiple machine learning models to predict vaccine uptake (`xyz_vaccine` and `seasonal_vaccine`).
   - Selected the best-performing model based on evaluation metrics (ROC AUC score).
   - Fine-tuned model hyperparameters using cross-validation and grid search techniques.

4. **Model Evaluation and Finalization:**
   - Finalized the model selection process and trained the best model on the entire training dataset.
   - Generated predictions for vaccine uptake on the test set (`test_set_features.csv`).

5. **Submission:**
   - Created a submission file (`submissions.csv`) containing predictions.
   - Ensured the format and contents of the submission file met competition or project requirements.

## Files Included
- **Notebook:** `Codefile.ipynb` - Jupyter Notebook containing the entire data preprocessing, modeling, and evaluation pipeline.
- **Submission File:** `submission.csv` - CSV file containing predictions for `respondent_id`, `h1n1_vaccine`, and `seasonal_vaccine`.
