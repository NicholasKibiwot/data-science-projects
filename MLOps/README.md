# MLOps - California Housing Prediction

## 📋 Project Overview

This project implements an end-to-end machine learning workflow for predicting housing prices using the California Housing dataset. The focus is on applying key MLOps concepts: preprocessing, cross-validation, hyperparameter tuning, pipeline construction, and model deployment.

## 🎯 Objectives

- Build a robust ML pipeline with proper preprocessing
- Implement hyperparameter tuning using GridSearchCV
- Evaluate model performance with cross-validation
- Serialize and deploy trained models
- (Optional) Create a REST API for model predictions

## 📊 Dataset

**Dataset Name:** California Housing (1990 Census)  
**Source:** scikit-learn `fetch_california_housing()`  
**Target Variable:** Median house value (in $100,000s)  
**Total Samples:** 20,640  
**Features:** 8  

### Features
- `MedInc`: Median income in block group
- `HouseAge`: Median house age in block group
- `AveRooms`: Average number of rooms per household
- `AveBedrms`: Average number of bedrooms per household
- `Population`: Block group population
- `AveOccup`: Average number of household members
- `Latitude`: Block group latitude
- `Longitude`: Block group longitude

## 🛠️ Technologies & Libraries

- **Python 3.8+**
- **scikit-learn:** ML algorithms and model selection tools
- **pandas:** Data manipulation
- **NumPy:** Numerical computing
- **Matplotlib/Seaborn:** Data visualization
- **Jupyter Notebook:** Interactive development
- **Kaggle:** Notebook deployment platform

## 🔄 Pipeline Architecture

```
Raw Data
   ↓
[Data Loading]
   ↓
[Preprocessing]
   ├─ Imputation (SimpleImputer)
   └─ Scaling (StandardScaler)
   ↓
[Train-Test Split] (80/20)
   ↓
[Model: KNeighborsRegressor]
   ↓
[GridSearchCV with 5-fold CV]
   ├─ n_neighbors: [3, 5, 7, 9]
   ├─ weights: ['uniform', 'distance']
   └─ p: [1, 2]
   ↓
[Model Evaluation]
   ├─ R² Score
   ├─ MSE
   └─ RMSE
   ↓
[Model Serialization] (pickle)
   ↓
[Deployment]
```

## 📈 Model Details

**Algorithm:** K-Nearest Neighbors Regressor  
**Validation Strategy:** 5-fold Cross-Validation  
**Hyperparameter Grid:**
- n_neighbors: [3, 5, 7, 9]
- weights: ['uniform', 'distance']
- p: [1, 2]

**Evaluation Metrics:**
- R² Score (coefficient of determination)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

## 📚 Key Learnings

- Data preprocessing and feature scaling importance
- Hyperparameter tuning strategies
- Cross-validation for robust model evaluation
- Pipeline construction for reproducibility
- Model serialization for deployment
- MLOps best practices

## 🔗 Links

- **Kaggle Notebook:** [MLOps Assignment](https://www.kaggle.com/code/nicholaskibiwot254/assignment-9-mlops)
- **Course Assignment:** [CyberShujaa Assignment 9](https://learning.cybershujaa.co.ke/mod/assign/view.php?id=2968)
- **Repository:** [data-science-projects](https://github.com/NicholasKibiwot/data-science-projects)

## ✅ Completion Status

- [x] Data Loading and Exploration
- [x] Preprocessing Pipeline
- [x] Train-Test Split
- [x] Model Definition
- [x] Hyperparameter Tuning (GridSearchCV)
- [x] Cross-Validation (5-fold)
- [x] Model Evaluation
- [x] Model Serialization
- [ ] API Deployment (Optional)

## 📝 Author

**Name:** Nicholas Kibiwot  
**GitHub:** [NicholasKibiwot](https://github.com/NicholasKibiwot)  
**Kaggle:** [nicholaskibiwot254](https://www.kaggle.com/nicholaskibiwot254)  

## 📄 License

This project is part of coursework and is available under the MIT License.

---

**Last Updated:** November 17, 2025  
**Status:** Completed
