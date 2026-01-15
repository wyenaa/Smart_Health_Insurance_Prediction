# 🏥 Smart Health Insurance Prediction

![Python](https://img.shields.io/badge/Python-3.12%2B-blue)
![Library](https://img.shields.io/badge/Library-Scikit--Learn%20%7C%20Pandas%20%7C%20Seaborn-green)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Regression-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

##  Project Overview
**Smart Health Insurance Prediction** is a Machine Learning project designed to predict individual medical insurance costs based on various demographic and health factors. 

By leveraging regression algorithms, this model helps insurance companies automate the underwriting process, ensuring fair premium pricing based on risk factors such as BMI, smoking habits, and age.

## Business Understanding
* **Problem:** Manual estimation of insurance premiums can be inconsistent and time-consuming.
* **Goal:** Build a predictive model to estimate medical costs accurately.
* **Value:**  **For Insurers:** Improved profitability and risk assessment.
    * **For Customers:** Transparent and fair pricing mechanisms.

## Dataset Description
The dataset consists of **1,338 rows** and **7 columns**. The target variable is `charges` (individual medical costs billed by health insurance).

| Column | Description | Type |
| :--- | :--- | :--- |
| `age` | Age of primary beneficiary | Numerical |
| `sex` | Insurance contractor gender (female, male) | Categorical |
| `bmi` | Body mass index ($kg/m^2$) | Numerical |
| `children` | Number of children covered by health insurance | Numerical |
| `smoker` | Smoking status (yes, no) | Categorical |
| `region` | Residential area in the US (ne, nw, se, sw) | Categorical |
| `charges` | Individual medical costs billed by health insurance | **Target (Numerical)** |

## Tech Stack & Methodology
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn

### Project Pipeline:
1.  **Exploratory Data Analysis (EDA):** Analyzing distributions, correlations, and detecting outliers.
2.  **Data Preprocessing:**
    * **Encoding:** Converting categorical variables (`sex`, `smoker`, `region`) using One-Hot Encoding/Label Encoding.
    * **Scaling:** Applying `MinMaxScaler` or `StandardScaler` to numerical features (`age`, `bmi`) to improve model convergence.
3.  **Model Building:** Experimenting with various regression algorithms:
    * Linear Regression
    * Random Forest Regressor
    * Gradient Boosting (XGBoost/LightGBM)
4.  **Evaluation:** Using metrics like $R^2$ Score, MAE (Mean Absolute Error), and RMSE.

## Key Insights & Results
*(Update this section with your specific findings)*

* **Smokers pay significantly more:** The correlation analysis shows a strong positive relationship between smoking status and charges.
* **Age factor:** Medical costs tend to increase with age.
* **BMI impact:** High BMI combined with smoking leads to the highest insurance charges.

### Model Performance:
| Model | R2 Score |
| :--- | :--- |
| Linear Regression | 0.75 |
| Random Forest Regressor | **0.86** (Best Model) |
| Decision Tree | 0.72 |

*> **Conclusion:** The Random Forest model provided the best accuracy in predicting insurance charges.*

##  How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/wyenaa/Smart_Health_Insurance_Prediction.git](https://github.com/wyenaa/Smart_Health_Insurance_Prediction.git)
    ```
2.  **Navigate to the directory:**
    ```bash
    cd Smart_Health_Insurance_Prediction
    ```
3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Run the Notebook:**
    Open `notebook.ipynb` (or your specific filename) in Jupyter Notebook or Google Colab.

## Contribution
Contributions are welcome! If you have suggestions for improving the model accuracy or feature engineering, feel free to open an issue or submit a pull request.

## 👤 Author
**Wyena (Suilianty** *Information Technology Student @ Brawijaya University* [LinkedIn](https://www.linkedin.com/in/wyena-suilianty) | [GitHub](https://github.com/wyenaa)

---
