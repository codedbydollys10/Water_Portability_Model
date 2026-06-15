# 💧 Water Potability Prediction Using Machine Learning

## 📌 Project Overview

Access to clean and safe drinking water is one of the most critical public health requirements worldwide. Water quality is determined by multiple physicochemical properties, making manual assessment time-consuming and resource-intensive.

This project leverages **Machine Learning** techniques to predict whether water is **safe for human consumption (Potable)** based on various water quality parameters.

The project includes:

* Exploratory Data Analysis (EDA)
* Data Cleaning and Missing Value Handling
* Feature Scaling and Standardization
* Class Imbalance Handling using SMOTE
* Machine Learning Model Training
* Performance Evaluation and Comparison
* Feature Importance Analysis
* Visualization and Insights

---

## 🎯 Objectives

The primary objectives of this project are:

* Analyze water quality data and identify important patterns.
* Handle missing values and data inconsistencies.
* Address class imbalance issues using SMOTE.
* Train multiple machine learning models.
* Compare model performance using multiple evaluation metrics.
* Identify the most influential factors affecting water potability.
* Build a reliable predictive system for water quality assessment.

---

## 📊 Dataset Information

The project uses the **Water Potability Dataset** containing various water quality measurements.

### Features

| Feature         | Description                                    |
| --------------- | ---------------------------------------------- |
| pH              | pH value of water                              |
| Hardness        | Water hardness level                           |
| Solids          | Total dissolved solids                         |
| Chloramines     | Chloramine concentration                       |
| Sulfate         | Sulfate concentration                          |
| Conductivity    | Electrical conductivity                        |
| Organic_carbon  | Organic carbon concentration                   |
| Trihalomethanes | THM concentration                              |
| Turbidity       | Water turbidity                                |
| Potability      | Target Variable (0 = Not Potable, 1 = Potable) |

### Target Variable

| Value | Meaning           |
| ----- | ----------------- |
| 0     | Non-Potable Water |
| 1     | Potable Water     |

---

## 🔍 Exploratory Data Analysis

Several exploratory techniques were applied:

* Dataset structure inspection
* Missing value analysis
* Statistical summary generation
* Distribution visualization
* Correlation analysis
* Boxplot analysis
* Target class distribution analysis

### Visualizations Included

* Feature Distributions
* Correlation Heatmap
* Class Distribution
* Boxplots
* ROC Curves
* Confusion Matrices
* Feature Importance Charts

---

## 🧹 Data Preprocessing

### Missing Value Treatment

Missing values were handled using:

```python
df.fillna(df.mean(), inplace=True)
```

Mean imputation was applied to preserve dataset size and avoid unnecessary data loss.

### Feature Scaling

The dataset was standardized using:

```python
StandardScaler()
```

This ensures that all features contribute equally to model training.

### Class Imbalance Handling

The dataset contains class imbalance between potable and non-potable samples.

To address this issue:

```python
SMOTE (Synthetic Minority Oversampling Technique)
```

was applied to generate synthetic samples for the minority class.

---

## 🤖 Machine Learning Models Used

### 1. Logistic Regression

A simple yet effective linear classification algorithm used as a baseline model.

**Advantages:**

* Fast training
* Highly interpretable
* Good baseline performance

---

### 2. Random Forest Classifiers

An ensemble learning method that combines multiple decision trees.

**Advantages:**

* Handles nonlinear relationships
* Robust against overfitting
* Provides feature importance

---

### 3. XGBoost Classifier

An advanced gradient boosting algorithm known for superior predictive performance.

**Advantages:**

* High accuracy
* Efficient learning
* Excellent handling of complex datasets

---

## 📈 Evaluation Metrics

Models were evaluated using:

### Accuracy

Measures overall prediction correctness.

### Precision

Measures the proportion of positive predictions that are actually correct.

### Recall

Measures the ability to correctly identify potable water samples.

### F1-Score

Harmonic mean of Precision and Recall.

### ROC-AUC Score

Measures model discrimination capability.

---

## 📉 Performance Comparison

The following metrics are compared across all models:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC

Performance visualizations include:

* Metric Comparison Graphs
* ROC Curves
* Confusion Matrices

---

## 🔬 Feature Importance Analysis

Feature importance was extracted from:

* Random Forest
* XGBoost

A combined importance score was computed to identify the most influential water quality parameters.

This helps understand:

* Which features most affect water potability
* How water quality can be monitored more effectively
* Key indicators for water treatment decisions

---

## 🛠️ Technologies Used

### Programming Language

* Python

### Data Analysis

* Pandas
* NumPy

### Data Visualization

* Matplotlib
* Seaborn

### Machine Learning

* Scikit-Learn
* XGBoost
* Imbalanced-Learn (SMOTE)

### Development Environment

* Google Colab
* Jupyter Notebook

---

## 📂 Project Structure

```text
Water_Portability_Model/
│
├── Water potability model.ipynb
├── water_potability.csv
├── Water potability model.py
└── README.md
```

---

## 🚀 How to Run

### Clone Repository

```bash
git clone https://github.com/codedbydollys10/Water_Portability_Model.git
```

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn
```

### Run Notebook

Open:

```text
Water potability model.ipynb
```

and execute all cells.

---

## 🌍 Real-World Applications

This project can be applied in:

### Public Health Monitoring

Rapid assessment of drinking water quality.

### Water Treatment Plants

Continuous monitoring and prediction of water safety.

### Environmental Research

Data-driven analysis of water resources.

### Smart Water Management Systems

Integration into automated water quality monitoring pipelines.

---

## 📌 Key Outcomes

✔ Successfully handled missing values

✔ Addressed class imbalance using SMOTE

✔ Trained multiple machine learning models

✔ Compared performance using multiple metrics

✔ Identified important water quality parameters

✔ Generated actionable insights for water safety assessment

---

## 🔮 Future Improvements

Potential enhancements include:

* Hyperparameter Optimization
* Cross-Validation
* Deep Learning Models
* Deployment as a Web Application
* Real-Time Water Monitoring Integration
* Explainable AI (SHAP/LIME)

---

## 👩‍💻 Author

**Dolly Sharma**

GitHub: https://github.com/codedbydollys10

---

## ⭐ Support

If you found this project useful, consider giving the repository a ⭐ on GitHub.
