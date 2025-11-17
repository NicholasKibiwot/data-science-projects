# Data Science Projects

A comprehensive collection of data science projects, coursework assignments, and portfolio work focusing on machine learning, data analysis, MLOps, and data engineering.

## 📚 Projects

### 1. Assignment 9: MLOps - California Housing Prediction
**Status:** Active  
**Framework:** Python, scikit-learn  
**Deployment:** Kaggle Notebook  

An end-to-end machine learning workflow implementing MLOps best practices to predict housing prices using the California Housing dataset.

**Key Features:**
- Data preprocessing using `ColumnTransformer`
- KNeighborsRegressor with hyperparameter tuning
- GridSearchCV with 5-fold cross-validation
- Hyperparameter optimization for: `n_neighbors` [3, 5, 7, 9], `weights` ['uniform', 'distance'], `p` [1, 2]
- Model evaluation with R² Score and RMSE
- Pipeline serialization with pickle
- Optional Flask/FastAPI deployment

**Dataset:** California Housing (1990 Census)  
**Target Variable:** Median house value (in $100,000s)  
**Features:** 8 (MedInc, HouseAge, AveRooms, AveBedrms, Population, AveOccup, Latitude, Longitude)

**Links:**
- [Kaggle Notebook](https://www.kaggle.com/code/nicholaskibiwot254/assignment-9-mlops)
- [Course Assignment](https://learning.cybershujaa.co.ke/mod/assign/view.php?id=2968)

## 🛠️ Technologies & Tools

**Programming Languages:**
- Python 3.8+
- SQL

**Libraries & Frameworks:**
- scikit-learn
- pandas
- NumPy
- Matplotlib & Seaborn
- Flask/FastAPI (for deployment)
- Jupyter Notebooks

**Platforms:**
- Kaggle Notebooks
- Google Colab
- GitHub

## 📖 Getting Started

### Prerequisites
```bash
Python 3.8+
pip install -r requirements.txt
```

### Installation
```bash
git clone https://github.com/NicholasKibiwot/data-science-projects.git
cd data-science-projects
```

## 📁 Repository Structure

```
data-science-projects/
├── README.md
├── requirements.txt
├── Assignment_9_MLOps/
│   ├── california_housing_mlops.ipynb
│   ├── california_knn_pipeline.pkl
│   ├── model_report.pdf
│   └── README.md
└── datasets/
    └── (datasets stored separately)
```

## 🎓 Learning Focus Areas

- **Machine Learning Models:** Regression, Classification, KNN, Linear Regression
- **Data Preprocessing:** Feature scaling, imputation, transformation
- **Cross-Validation:** 5-fold CV, GridSearchCV, hyperparameter tuning
- **Model Evaluation:** R² Score, MSE, RMSE, classification metrics
- **MLOps Practices:** Model serialization, versioning, deployment
- **Data Analysis & Visualization:** EDA, matplotlib, seaborn
- **Data Wrangling:** Cleaning, transformation, feature engineering

## 📊 Project Statistics

- **Total Projects:** 1 (Growing)
- **Primary Framework:** Python + scikit-learn
- **Estimated Hours:** 40+ hours of coursework

## 🔗 Quick Links

- **GitHub Profile:** [NicholasKibiwot](https://github.com/NicholasKibiwot)
- **Kaggle Profile:** [nicholaskibiwot254](https://www.kaggle.com/nicholaskibiwot254)
- **Course Platform:** [CyberShujaa](https://learning.cybershujaa.co.ke)

## 📝 License

This repository is open source and available under the MIT License. See LICENSE file for details.

## 🤝 Contributing

This is a personal portfolio and coursework repository. Contributions are not currently accepted.

## 📧 Contact

For inquiries or feedback, please reach out through GitHub or email.

---

**Last Updated:** November 17, 2025  
**Status:** Actively updating with new projects and coursework
