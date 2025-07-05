# 🧬 Lung Cancer Risk Prediction Using Random Forest Classifier on Survey Data

This project applies a Random Forest classification model to predict the likelihood of lung cancer based on survey data. It includes exploratory data analysis, preprocessing, outlier detection, label encoding, and model evaluation.

---

## 📁 Dataset

- **Name**: `survey lung cancer.csv`
- **Source**: [UCI Repository / Kaggle / Medical Surveys]
- **Features**:
  - Demographic: `AGE`, `GENDER`
  - Behavioral & Symptomatic: `SMOKING`, `ANXIETY`, `ALCOHOL CONSUMING`, `COUGHING`, etc.
- **Target**: `LUNG_CANCER` (Label indicating presence or absence)

---

## 🧪 Objective

To develop a predictive model that can:
- Classify individuals at risk of lung cancer using survey data
- Compare predictions with actual outcomes using confusion matrix and accuracy
- Detect outliers and clean the dataset before model training

---

## 🔧 Tools & Technologies

- **Python 3.11+**
- **Pandas & NumPy** – Data loading & manipulation
- **Missingno** – Visualizing missing data
- **Seaborn & Matplotlib** – Data visualization
- **Scikit-learn** – Preprocessing, modeling, evaluation

---

## 📈 Workflow Summary

### ✅ Data Preprocessing
- Checked for missing values using `missingno.matrix`
- Encoded categorical features (`GENDER`, `LUNG_CANCER`) using `LabelEncoder`
- Detected outliers in `AGE` column using **Z-score method**

### ✅ Model Building
- Split the dataset into training and testing sets (90/10)
- Trained a **Random Forest Classifier** with:
  - 1000 trees
  - `max_depth=5`
  - `n_jobs=-1` for parallel processing
- Evaluated using:
  - Accuracy Score
  - Confusion Matrix

---

## 🧠 Model Performance

| Metric         | Value        |
|----------------|--------------|
| Model Used     | RandomForestClassifier |
| Accuracy       | ✅ *Displayed in output* |
| Confusion Matrix | ✅ *Displayed in output* |

> The model shows good performance in identifying potential lung cancer cases based on symptoms and lifestyle patterns.

---
