# Residential Real Estate Valuation & Price Prediction - Architecture & Pipeline Design

```mermaid
graph TD
    DataInput[Raw CSV Dataset: predicting house price.csv] --> Preproc[Data Cleaning & Column Transformer]
    Preproc -->|Numeric| Scaler[StandardScaler Normalization]
    Preproc -->|Categorical| Encoder[One-Hot Categorical Encoding]
    Scaler --> Split[Train/Test Stratified Split 80/20]
    Encoder --> Split
    Split --> Train[Model Training: Gradient Boosting Regressor]
    Train --> Eval[Evaluation & Benchmarks]
    Eval --> Inference[Production Inference & CLI]
```

## Comparative Models Evaluated
- **Gradient Boosting Regressor**
- **Random Forest Regressor**
- **Ridge Regression**
- **XGBoost Regressor**
