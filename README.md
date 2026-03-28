# Machine Learning Group Assignment

## Extreme Rainfall Risk Classification for Sri Lankan Cities

## 📌 Project Overview

This project focuses on the **evaluation and comparison of classical machine learning models**
to classify **rainfall intensity levels in Sri Lankan cities** using a real-world weather dataset.

The system applies **supervised machine learning (multi-class classification)** techniques
to predict rainfall categories based on historical weather conditions such as temperature,
wind speed, radiation, and atmospheric measurements.

The objective is to support **weather analysis, disaster preparedness, and decision-making**
by providing a data-driven classification of rainfall levels.

---

## 🎯 Problem Statement

Unpredictable rainfall patterns in Sri Lanka can lead to floods, transportation disruptions,
and agricultural losses. Therefore, accurately identifying rainfall intensity levels is crucial.

This project classifies rainfall into four categories:

* **No Rain**
* **Light Rain**
* **Moderate Rain**
* **Heavy Rain**

---

## 📊 Dataset

* Dataset: Sri Lanka Weather Dataset
* Records: ~147,000
* Features: 20+
* Coverage: 30 cities across Sri Lanka

The dataset includes:

* Temperature (min, max, mean)
* Apparent temperature
* Rainfall measurements
* Wind speed and gusts
* Solar radiation
* Sunrise and sunset times
* Elevation and location

---

## ⚙️ Methodology

### 1. Data Preprocessing

* Handling missing values
* Feature engineering (date-based features, day length)
* Encoding categorical variables
* Removal of data leakage features

### 2. Target Variable Creation

Rainfall intensity is categorized based on `rain_sum`:

* `0` → No Rain
* `0 < rain_sum < 5` → Light Rain
* `5 ≤ rain_sum < 20` → Moderate Rain
* `rain_sum ≥ 20` → Heavy Rain

### 3. Models Used

The following machine learning models were implemented and compared:

* Logistic Regression
* Decision Tree
* Random Forest
* K-Nearest Neighbors (KNN)

---

## 📈 Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

---

## 📊 Results

The models were compared based on their performance metrics.

* Random Forest achieved the best overall performance
* Decision Tree showed good interpretability
* Logistic Regression provided a strong baseline
* KNN performance depended on distance scaling

---

## 📁 Project Structure

```
ML-Rainfall-Prediction/
│
├── data/
│   ├── raw/
│   ├── processed/
│
├── notebooks/
│   ├── 01_preprocessing.ipynb
│   ├── 02_logistic_regression.ipynb
│   ├── 03_decision_tree.ipynb
│   ├── 04_random_forest.ipynb
│   ├── 05_knn.ipynb
│   ├── 06_model_comparison.ipynb
│
├── models/
├── reports/
├── src/
│
├── README.md
├── requirements.txt
```

---

## 🚀 Future Improvements

* Hyperparameter tuning for improved accuracy
* Integration with real-time weather data
* Deployment as a web-based prediction system
* Extension to time-series forecasting

---

## 👥 Team Contribution

Each team member contributed by implementing and evaluating different machine learning models,
ensuring a fair comparison and collaborative development.

---

## 📌 Conclusion

This project demonstrates how classical machine learning techniques can be effectively used
to classify rainfall intensity levels using real-world data. The results highlight the importance
of proper preprocessing, feature engineering, and model selection in achieving reliable predictions.
