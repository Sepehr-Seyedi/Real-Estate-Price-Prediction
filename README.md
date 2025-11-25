
---

# 🏡 Real Estate Price Analysis

Comprehensive Data Exploration, Statistical Testing & Predictive Modeling

## 📌 Overview

This project analyzes real estate pricing data to uncover the factors that influence the *house price of unit area*. It includes full data cleaning, exploration, visualization, statistical analysis, and a linear regression model.
The project aims to understand how variables such as **house age**, **distance to MRT**, **number of convenience stores**, **latitude**, and **longitude** impact real estate prices.

## 📁 Project Structure

```
repo/
 ├── src/
 │    └── main.py                # Main analysis script
 ├── README.md                   # Project documentation
 ├── requirements.txt            # Python dependencies
 ├── LICENSE                     # MIT License
 ├── .gitignore                  # Ignored files for Git
```

## 📊 Key Features

### ✔ **Data Cleaning**

* Removed irrelevant columns
* Renamed features for clarity
* Addressed missing values
* Identified and removed extreme outliers based on:

  * House price
  * MRT distance
  * Longitude

### ✔ **Exploratory Data Analysis (EDA)**

Includes various visualizations:

* Line plots showing relationships with housing prices
* Distribution plots (histograms + KDE)
* Boxplots detecting outliers
* Correlation heatmap
* Scatter plots for predicted vs actual values

### ✔ **Statistical Analysis**

Hypothesis testing performed:

* **T-test:** Difference in price based on above/below median house age
* **ANOVA:** Price differences across number of convenience stores
* **Chi-square test:** Association between transaction date and convenience store count
* Correlation calculations for key features

### ✔ **Machine Learning Model**

A **Linear Regression** model is trained to predict unit price based on all numerical features.

Evaluation metrics:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² score

## 🚀 How to Run the Project

### 1️⃣ **Clone the Repository**

```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
```

### 2️⃣ **Install Dependencies**

```bash
pip install -r requirements.txt
```

### 3️⃣ **Run the Analysis**

```bash
python src/main.py
```

## 📦 Dependencies

All required packages are listed in `requirements.txt`, including:

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* SciPy

## 📈 Results & Insights

* Housing prices increase when **closer to MRT stations**
* More **convenience stores nearby** → higher prices
* House age shows **non-linear effects**
* Certain lat/long regions show price clusters
* Regression model provides interpretable coefficients to quantify these effects

## 📜 License

This project is released under the **MIT License**.
Feel free to use, modify, and distribute it.

## 🙌 Acknowledgments

Dataset source: *Real Estate Valuation Data Set*
Analysis code provided originally in Jupyter format and refactored into production-ready Python script.

---

