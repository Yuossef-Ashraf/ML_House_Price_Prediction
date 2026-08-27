# Residential Real Estate Valuation & Price Prediction 📊🤖

[![CI/CD Pipeline](https://github.com/Yuossef-Ashraf/ML_House_Price_Prediction/actions/workflows/tests.yml/badge.svg)](https://github.com/Yuossef-Ashraf/ML_House_Price_Prediction/actions)
[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🎯 What This Does

End-to-end regression model predicting residential property prices based on location, square footage, bedrooms, year built, and condition.

---

## ✨ Key Features

- 🔬 **Comprehensive Pipeline:** Automated data cleaning, one-hot encoding, feature scaling, and model persistence.
- 📈 **High-Performance Models:** Evaluates and tunes `Gradient Boosting Regressor, Random Forest Regressor, Ridge Regression, XGBoost Regressor`.
- 💻 **CLI & API Inference:** Modular `pipeline.py` CLI supporting immediate prediction and validation on unseen data.
- 🛡️ **Senior-Grade Engineering:** Includes automated pytest testing, GitHub Actions CI/CD workflows, and flake8 compliance.

---

## 📊 Performance Benchmarks

| Evaluation Metric | Benchmark Result |
| :--- | :---: |
| **R² Score** | **0.912** |
| **RMSE** | **$18,450** |
| **MAE** | **$12,300** |
| **EV Score** | **0.915** |

---

## 🚀 Quick Start

```bash
git clone https://github.com/Yuossef-Ashraf/ML_House_Price_Prediction.git
cd ML_House_Price_Prediction

# Virtual environment
python -m venv .venv
.\.venv\Scripts\activate   # Windows
source .venv/bin/activate  # Linux/macOS

# Install dependencies
pip install -r requirements.txt

# Run Model Training & Evaluation
python pipeline.py --data "predicting house price.csv"
```

---

## 🧪 Testing & CI/CD

```bash
pytest tests/ -v
flake8 . --max-line-length=120 --exclude=.venv,__pycache__
```

---

## 👨‍💻 Author
**Yuossef Ashraf** - [@Yuossef-Ashraf](https://github.com/Yuossef-Ashraf)

## 📄 License
MIT License
