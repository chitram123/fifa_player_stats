#  Player Value Prediction using Machine Learning

##  Project Overview

This project aims to predict the **market value of football players** using machine learning techniques based on their physical, technical, and performance attributes.

The project also explores:

* Impact of **log transformation**
* Effect of **PCA (dimensionality reduction)**
* Improvement using **hyperparameter tuning (GridSearchCV)**

---

##  Dataset

The dataset includes:

* Player information (player, club, country)
* Physical attributes (age, height, weight)
* Technical skills (passing, dribbling, tackling, etc.)
* Performance metrics
* Target variable: **Player Value**

---

##  Exploratory Data Analysis (EDA)

* Removed irrelevant and high-cardinality features
* Handled missing values (`marking` column dropped)
* Converted `value` from string to numeric
* Identified skewness in target variable
* Performed univariate and bivariate analysis

---

##  Data Preprocessing

* Feature selection applied
* Data scaling where required
* Target variable transformation using log

---

##  Dimensionality Reduction (PCA)

* Applied PCA to reduce feature dimensions
* Selected components based on 95% variance
* Observed that PCA did not improve model performance

---

##  Model Building

* Baseline model: Random Forest Regressor
* Improved model using log-transformed target

---

##  Hyperparameter Tuning

Used GridSearchCV to find optimal parameters:

* n_estimators = 100
* max_depth = None
* min_samples_split = 5

---

##  Model Performance

| Model                 | R² Score | Remarks              |
| --------------------- | -------- | -------------------- |
| Baseline Model        | 0.70     | Good performance     |
| Log Transformed Model | 0.78     | Improved learning    |
| Tuned Model           | 0.78     | Stable and optimized |

**Cross-validation score: 0.76**

---

##  Key Insights

* Player value is influenced by technical and physical attributes
* Log transformation helped handle skewed data
* Hyperparameter tuning improved model stability

---

## Conclusion

The final model achieved:

* **R² Score: 0.78**
* **Cross-validation Score: 0.76**

The model demonstrates strong predictive capability and generalization.

---

## Future Improvements

* Use advanced models (XGBoost, LightGBM)
* Include categorical feature encoding
* Perform feature engineering
* Apply advanced outlier handling techniques

---

## Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

---



---
