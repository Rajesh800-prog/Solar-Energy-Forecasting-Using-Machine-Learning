# ☀️ Solar Energy Forecasting Using Machine Learning



---

## 📌 About This Project

Solar panels produce electricity from sunlight — but the amount changes every day depending on weather.  
This project uses **Machine Learning** to predict how much solar power will be generated, helping power companies plan better and avoid electricity shortages.

---

## 🎯 Objective

- Predict solar power generation using real weather and solar data
- Compare 9 different machine learning models
- Find the best model with highest accuracy
- Identify which weather factors affect solar power the most

---

## 📂 Dataset

- **Source:** [Solar Energy Power Generation Dataset — Kaggle](https://www.kaggle.com/datasets/stucom/solar-energy-power-generation-dataset)
- **Rows:** 68,778 records
- **Columns:** DATE_TIME, PLANT_ID, SOURCE_KEY, DC_POWER, AC_POWER, DAILY_YIELD, TOTAL_YIELD
- **Target Variable:** AC_POWER (solar power generated in kW)

---

## 🤖 Machine Learning Models Used

| Model | Type | R² Score |
|-------|------|----------|
| Multiple Linear Regression | Classical | 0.60 |
| Ridge Regression | Classical | 0.73 |
| LASSO Regression | Classical | 0.73 |
| Decision Tree Regression | Classical | 0.75 |
| Support Vector Regression | Classical | 0.39 |
| Random Forest Regression | Ensemble | 0.82 |
| Bagging Regressor | Ensemble | 0.81 |
| AdaBoost Regressor | Ensemble | 0.69 |
| **Gradient Boosting Regressor** | **Ensemble** | **0.83 ✅ BEST** |

---

## 🏆 Best Model Result

```
Model  : Gradient Boosting Regressor
R²     : 0.827  (82.7% accuracy)
RMSE   : 399.44
MAE    : 253.62
```

---

## 🔑 Key Findings

- ✅ **Gradient Boosting Regressor** gave the best predictions
- ✅ **Sun position** (zenith angle, azimuth, angle of incidence) are the most important features
- ✅ **Ensemble models** always perform better than single models
- ✅ Hyperparameter tuning improved accuracy by **4.4%**

---

## 🛠️ Tools and Technologies

| Tool | Purpose |
|------|---------|
| Python 3 | Programming language |
| Google Colab | Cloud notebook to run code |
| Pandas | Data loading and cleaning |
| NumPy | Mathematical calculations |
| Scikit-learn | Machine learning models |
| Matplotlib & Seaborn | Charts and visualizations |

---

## 📊 Project Steps

1. Load and explore the dataset (EDA)
2. Data preprocessing and feature engineering
3. Train 5 classical ML models
4. Train 4 ensemble ML models
5. Hyperparameter tuning with Grid Search
6. 5-Fold Cross Validation
7. Compare all models and find the best one
8. Plot results and feature importance

---

## 🚀 How to Run

1. Open the notebook in Google Colab:  
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

2. Upload the Kaggle CSV dataset when prompted

3. Click **Runtime → Run All**

4. View all results and charts automatically!

---

## 📁 Files in This Repository

```
solar-energy-forecasting/
│
├── Solar_Energy_Forecasting_Colab.ipynb   ← Main notebook (run this)
├── README.md                              ← Project description
```

---

## 👨‍🎓 Project Info

- **Project Type:** Mini Project / Academic
- **Domain:** Renewable Energy + Machine Learning
- **Reference Paper:** IEEE Access, Volume 13, 2025
- **Tools:** Python, Scikit-learn, Google Colab
