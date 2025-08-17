```markdown
# Credit Risk Prediction Project

This project delivers a machine learning solution for predicting loan default risk, designed for financial institutions such as Bank of Scotland. The implementation adheres to Financial Conduct Authority (FCA) regulations, emphasizing model transparency, fairness, and auditability to meet industry standards for credit risk analytics.

## Overview
The project processes loan application data to predict default probabilities, leveraging a robust pipeline that includes data preprocessing, model training, hyperparameter tuning, evaluation, and interpretability. A Streamlit-based interface enables interactive predictions for demonstration purposes, while the codebase is structured for secure deployment in production environments.

## Key Features
- **Data Preprocessing**: Handles missing values and categorical features using a scalable pipeline with median imputation and one-hot encoding.
- **Model Development**: Implements Logistic Regression, Random Forest, and XGBoost models, with stratified k-fold cross-validation to address class imbalance (~8% default rate).
- **Hyperparameter Tuning**: Optimizes models using RandomizedSearchCV, achieving AUC-ROC ~0.7308 and AUC-PR ~0.1767 for the tuned XGBoost model, surpassing target thresholds (AUC-ROC > 0.70, AUC-PR > 0.16).
- **Interpretability**: Integrates SHAP for transparent feature importance analysis, ensuring compliance with FCA’s emphasis on explainable AI.
- **Fairness and Compliance**: Includes bias checks (e.g., gender-based default rates) to align with FCA fair lending requirements and GDPR data privacy standards.
- **Auditability**: Logs model training and predictions for regulatory oversight.
- **Demo Interface**: Provides a Streamlit app for interactive predictions, with production guidelines for secure API deployment.

## Technical Contributions
This project showcases advanced machine learning techniques applied to credit risk modeling, demonstrating expertise in:
- Building compliant, interpretable models for financial applications.
- Implementing robust preprocessing and evaluation pipelines for imbalanced datasets.
- Ensuring regulatory compliance through bias checks and audit logging.
- Developing user-friendly interfaces for stakeholder engagement.

## Installation
```bash
pip install -r requirements.txt
```

## Usage
1. Upload `application_train.csv` (excluded for data privacy compliance).
2. Run `credit_risk_prediction.py` in Google Colab or a Python environment.
3. For the Streamlit demo, replace `YOUR_TOKEN` with an ngrok authtoken and execute the script.

## Impact
The model achieves high predictive performance while maintaining transparency and fairness, making it suitable for real-world loan decision systems. Its compliance with FCA and GDPR standards positions it as a valuable tool for financial institutions seeking to balance risk management with regulatory obligations.

## License
MIT License
```