# 🔥 Algerian Forest Fire Prediction System using Machine Learning & AWS CI/CD

## 📌 Project Overview

Forest fires pose a serious threat to ecosystems, human life, and property.
This project builds an **end-to-end Machine Learning system** to predict the **Fire Weather Index (FWI)** using real-world meteorological data from Algeria. The solution covers **data preprocessing, exploratory data analysis, regression modeling, cross-validation, and cloud deployment** using AWS.

---

## 📊 Dataset Information

* **Dataset:** Algerian Forest Fires Dataset
* **Total Instances:** 244
* **Regions:**

  * Bejaia (Northeast Algeria) – 122 samples
  * Sidi Bel-Abbes (Northwest Algeria) – 122 samples
* **Time Period:** June 2012 – September 2012
* **Target Variable:** Fire Weather Index (FWI)

---

## 🧩 Features

**Weather Variables**

* Temperature
* Relative Humidity (RH)
* Wind Speed (Ws)
* Rainfall

**FWI Components**

* FFMC (Fine Fuel Moisture Code)
* DMC (Duff Moisture Code)
* DC (Drought Code)
* ISI (Initial Spread Index)
* BUI (Buildup Index)

---

## 🧹 Data Preprocessing

* Handled missing and inconsistent values
* Corrected data types and cleaned column names
* Encoded categorical variables
* Removed multicollinearity using **correlation-based feature selection**
* Standardized features using **StandardScaler**

---

## 📈 Exploratory Data Analysis (EDA)

* Analyzed seasonal fire trends across regions
* Identified **August and September** as peak fire months
* Visualized feature distributions, correlations, and outliers
* Used heatmaps, boxplots, histograms, and count plots

---

## 🤖 Machine Learning Models

The following regression models were implemented and evaluated:

* Linear Regression
* Ridge Regression (RidgeCV)
* Lasso Regression (LassoCV)
* ElasticNet Regression (ElasticNetCV)

All models were evaluated using **Mean Absolute Error (MAE)** and **R² Score**, with **5-fold cross-validation** for regularized models.

---

## 🏆 Model Performance

| Model                      | MAE  | R² Score |
| -------------------------- | ---- | -------- |
| Linear Regression          | 0.55 | 0.9848   |
| Ridge Regression (CV)      | 0.56 | 0.9843   |
| Lasso Regression (CV)      | 0.62 | 0.9821   |
| ElasticNet Regression (CV) | 0.66 | 0.9814   |

✅ **Best Performance:** Linear & Ridge Regression
✅ **Overall Accuracy:** ~98.4% R² with MAE < 0.6

---

## ☁️ Deployment & CI/CD

* Deployed the trained ML model using **AWS Elastic Beanstalk**
* Implemented **CI/CD pipeline** with **GitHub**
* Automated build, integration, and deployment on code push
* Configured AWS environment variables, IAM roles, and logging

---

## 🛠️ Tech Stack

* **Programming:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn
* **Machine Learning:** Regression, Regularization, Cross-Validation
* **Cloud & DevOps:** AWS Elastic Beanstalk, IAM, GitHub CI/CD
* **Version Control:** Git, GitHub

---

## 📂 Project Structure

```
├── data/
│   ├── Algerian_forest_fires_dataset_UPDATE.csv
│   └── Algerian_forest_fires_cleaned_dataset.csv
│
├── notebooks/
│   └── EDA_and_Modeling.ipynb
│
├── src/
│   └── model_training.py
│
├── requirements.txt
├── README.md
└── app.py
```

---

## 🚀 How to Run the Project

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/algerian-forest-fire-prediction.git
cd algerian-forest-fire-prediction
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Application

```bash
python app.py
```

---

## 📌 Key Learnings

* Built a complete ML pipeline from raw data to deployment
* Gained hands-on experience with **regularized regression models**
* Learned **feature selection, scaling, and cross-validation**
* Deployed a production-ready ML application using AWS & CI/CD

---

## 👨‍💻 Author

**Rajat Agrawal**
M.Tech (Machine Learning)
📌 Aspiring ML Engineer | Data Scientist

---

## ⭐ Acknowledgements

* UCI Machine Learning Repository
* Canadian Forest Fire Weather Index (FWI) System

---

### ⭐ If you like this project, consider giving it a star!

---


Just tell me 👍
