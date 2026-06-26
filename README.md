# Predict Calorie Expenditure

An end-to-end Machine Learning pipeline for predicting calorie expenditure using biometric and physiological data. The project leverages advanced feature engineering, ensemble learning, and deep learning techniques to model complex relationships between exercise attributes and energy expenditure.

---

## Project Overview

Accurately estimating calories burned during physical activity is important for fitness tracking, health monitoring, and personalized workout planning. Traditional estimation methods often struggle to capture complex physiological interactions.

This project develops and evaluates multiple Machine Learning and Deep Learning models to predict calorie expenditure using demographic, biometric, and exercise-related attributes. The solution includes extensive exploratory data analysis, feature engineering, model benchmarking, and performance evaluation.

---

## Dataset

| Metric | Value |
|----------|----------|
| Training Samples | 750,000 |
| Test Samples | 250,000 |
| Original Features | 7 |
| Engineered Features | 11 |
| Total Features Used | 18 |

### Input Features

- Age
- Gender
- Height
- Weight
- Duration
- Heart Rate
- Body Temperature

### Target Variable

- Calories Burned

---

## Project Workflow

```text
Raw Data
    ↓
Data Cleaning
    ↓
Exploratory Data Analysis
    ↓
Feature Engineering
    ↓
Feature Scaling
    ↓
Model Training
    ↓
Model Evaluation
    ↓
Prediction
```

---

## Exploratory Data Analysis

Performed extensive exploratory analysis to understand feature distributions, correlations, and relationships with calorie expenditure.

### Correlation Heatmap

<img width="613" height="545" alt="img3" src="https://github.com/user-attachments/assets/f0d89364-9e26-4ff6-8df3-49d0ede89386" />

The correlation heatmap highlights the relationships among physiological features and calorie expenditure, helping identify important predictors and guide feature engineering decisions.

### Key Analyses

- Correlation Heatmaps
- Distribution Analysis
- Outlier Detection
- Feature Relationship Visualization
- Target Variable Analysis

---

## Feature Engineering

Domain-specific features were engineered to improve predictive performance and capture physiological relationships.

### Engineered Features

- Body Mass Index (BMI)
- Heart Rate Zones
- Age Groups
- Duration × Heart Rate
- Age × Weight
- Additional physiological interaction features

These transformations expanded the feature space from 7 raw attributes to 18 informative features.

---

## Models Evaluated

The following models were trained and benchmarked:

| Model |
|---------|
| Linear Regression |
| ElasticNet Regression |
| XGBoost Regressor |
| LightGBM Regressor |
| Deep Neural Network (TensorFlow) |

---

## Results

### Best Performing Model

**XGBoost Regressor**

### Performance

| Metric | Value |
|----------|----------|
| RMSE | 3.60 Calories |

### Model Performance Comparison

<img width="696" height="394" alt="img" src="https://github.com/user-attachments/assets/bbb5beb1-eb2b-4d34-a51a-2d083d22f017" />


### Performance Evaluation - Computational Overhead

<img width="803" height="349" alt="img2" src="https://github.com/user-attachments/assets/9b750b34-22c7-4bf6-a7d2-29ed867f377a" />


### Key Findings

- Ensemble learning methods significantly outperformed linear models.
- XGBoost achieved the best overall predictive performance.
- Feature engineering substantially improved model accuracy.
- Physiological interaction features contributed strongly to prediction quality.

---

## Technologies Used

### Programming Language

- Python

### Libraries & Frameworks

- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- TensorFlow
- XGBoost
- LightGBM

### Development Environment

- Jupyter Notebook

---

## Repository Structure

```text
predict-calorie-expenditure/
│
├── notebooks/
│   └── predict_calorie_expenditure.ipynb
│
├── reports/
│   └── Project_Report.pdf
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## How to Run

### Clone Repository

```bash
git clone https://github.com/TanmayJindal1205/predict-calorie-expenditure.git
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Launch Notebook

```bash
jupyter notebook
```

Open:

```text
notebooks/predict_calorie_expenditure.ipynb
```

---

## Future Improvements

- Hyperparameter Optimization
- SHAP-based Explainability
- Real-Time Prediction API
- Streamlit Web Application
- Integration with Fitness Tracking Platforms
- Cloud Deployment

---

## Documentation

Detailed project documentation is available in:

```text
reports/Project_Report.pdf
```

---

## Author

**Tanmay Jindal**

Machine Learning • Deep Learning • Data Science
