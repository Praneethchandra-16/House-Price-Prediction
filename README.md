# 🏠 House Price Prediction - Regression Project

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0%2B-orange)
![Status](https://img.shields.io/badge/status-complete-brightgreen)

## 📘 Overview
A complete machine learning pipeline to predict house prices in California using the California Housing Dataset. Includes EDA, preprocessing, modeling, hyperparameter tuning, and evaluation.

---

## 📂 Project Structure
```
├── datasets
│   └── housing.csv
├── images
│   └── plots.png (auto-saved figures)
├── House_Price_Prediction.ipynb
└── README.md
```

---

## 📥 Data Collection
- Source: [Aurelien Geron's GitHub](https://github.com/ageron/data)
- Dataset: `housing.tgz` → extracted to `housing.csv`

---

## 🔍 Data Exploration
- `.info()`, `.describe()`, `.value_counts()`
- Visual inspection of distributions with `hist()`
- Feature `ocean_proximity` is categorical

---

## 📊 Visualizations
- Histograms for all features
- Scatter plot (longitude vs latitude)
- Correlation matrix & scatter matrix
- Bar plot for stratified income categories

---

## 🧹 Data Preprocessing
- Missing value imputation with `SimpleImputer`
- Custom attributes: `rooms_per_household`, `bedrooms_per_room`, etc.
- Categorical encoding: `OneHotEncoder`
- Feature scaling: `StandardScaler`
- Used `Pipeline` and `ColumnTransformer`

---

## 📈 Modeling
Models trained:
- ✅ Linear Regression
- ✅ Decision Tree Regressor
- ✅ Random Forest Regressor

**Evaluation:**
- RMSE (Root Mean Squared Error)
- `cross_val_score` with negative MSE
- GridSearchCV for hyperparameter tuning

---

## 🧪 Final Testing
- Evaluated final model (Random Forest) on test set
- Generated confidence intervals using `scipy.stats`

---

## 💡 Key Insights
- `median_income` is the most important feature
- Stratified sampling improved data splits
- Feature engineering improved model performance

---

## 🔧 Tools & Libraries
- Python 🐍
- Pandas, NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 🚀 Future Work
- ✅ Model deployment with **Flask**, **Streamlit**, or **FastAPI**
- ✅ Save model using `joblib`
- ✅ Track metrics using **MLflow** or **Weights & Biases**
- 📊 Add interactive visual dashboards

---

## 🙌 Acknowledgements
- Based on Chapter 2 of *Hands-On Machine Learning* by Aurelien Geron

---

> Made with ❤️ by Praneeth

