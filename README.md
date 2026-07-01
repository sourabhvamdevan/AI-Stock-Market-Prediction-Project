# AI-Powered Stock Market Trend Prediction using Machine Learning and FinBERT

## Overview

This project presents an AI-powered Stock Market Trend Prediction System that combines historical stock market data with financial sentiment analysis to predict market trends.

The system performs data preprocessing, exploratory data analysis, feature engineering, machine learning model training, and financial sentiment analysis using FinBERT. Multiple machine learning algorithms are evaluated to identify the most effective prediction model.

---

## Features

- Historical stock market data analysis
- Data preprocessing and cleaning
- Exploratory Data Analysis (EDA)
- Feature engineering
- Label encoding for categorical features
- Feature scaling using StandardScaler
- Financial sentiment analysis using FinBERT
- Comparison of multiple machine learning models
- Feature importance visualization
- Confusion matrix evaluation
- Model saving for future predictions

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- LightGBM
- Hugging Face Transformers
- FinBERT
- Joblib
- Google Colab / Jupyter Notebook

---

## Dataset Features

The dataset contains historical stock market information along with sentiment-related attributes.

Features include:

- Open Price
- High Price
- Low Price
- Close Price
- Adjusted Close Price
- Trading Volume
- Company
- Date
- Financial Score
- Sentiment Score
- Financial News Text
- Target Variable

---

## Project Workflow

```text
Dataset
    │
    ▼
Data Cleaning
    │
    ▼
Exploratory Data Analysis
    │
    ▼
Feature Engineering
    │
    ▼
Label Encoding
    │
    ▼
Feature Scaling
    │
    ▼
Train-Test Split
    │
    ▼
Machine Learning Models
    │
    ├── Logistic Regression
    ├── Decision Tree
    ├── Random Forest
    ├── Gradient Boosting
    ├── XGBoost
    └── LightGBM
    │
    ▼
Model Evaluation
    │
    ▼
Best Model Selection
    │
    ▼
Model Saving
```

---

## FinBERT Integration

Financial news text is processed using the pretrained **FinBERT** transformer model to generate:

- Financial sentiment labels
- Confidence scores

These generated features demonstrate how transformer-based financial NLP can be incorporated into stock market prediction pipelines.

Due to computational requirements, FinBERT inference is demonstrated on a representative subset of the dataset.

---

## Machine Learning Models

The following algorithms were implemented and evaluated:

- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- XGBoost
- LightGBM

---

## Model Performance

| Model | Accuracy |
|--------|----------|
| Logistic Regression | 61.97% |
| Decision Tree | 77.05% |
| Gradient Boosting | 76.39% |
| XGBoost | 81.07% |
| LightGBM | 83.76% |
| Random Forest | **91.30%** |

Random Forest achieved the highest prediction accuracy and was selected as the final model.

---

## Project Structure

```
AI-Stock-Market-Prediction/
│
├── AI_Stock_Market_Prediction.ipynb
├── stock_prediction_model.pkl
├── scaler.pkl
├── README.md
└── Dataset/
```

---

## Installation

Clone the repository.

```bash
git clone https://github.com/yourusername/AI-Stock-Market-Prediction.git
```

Install the required packages.

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm transformers torch joblib
```

Run the notebook.

```bash
jupyter notebook
```

or

```bash
Google Colab
```

---

## Results

- Successfully built a complete stock trend prediction pipeline.
- Compared six machine learning algorithms.
- Integrated transformer-based financial sentiment analysis using FinBERT.
- Evaluated models using confusion matrix and classification metrics.
- Saved the best-performing model for future prediction.

---

## Future Improvements

- Perform FinBERT inference on the complete dataset using GPU acceleration.
- Integrate live financial news feeds.
- Connect with Yahoo Finance API.
- Develop a Streamlit dashboard.
- Deploy the model using Flask or FastAPI.
- Explore LSTM and Transformer-based forecasting models.

---

## Author

**Sourabh Vamdevan**



