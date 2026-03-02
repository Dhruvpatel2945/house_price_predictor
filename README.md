# 🏠 King County House Price Predictor
> An end-to-end Regression project to predict real estate prices using Big Data Analytics techniques.

---

## 📊 Project Overview
This project predicts the sales price of houses in King County, USA. Instead of just running a basic model, I focused on **Feature Engineering** to transform raw data into meaningful predictors, helping the model understand the "logic" behind property valuation.

## 🛠️ The "Rich" Data Pipeline
To move beyond a basic student project, I implemented the following steps:

1.  **Exploratory Data Analysis (EDA):** Identified high-correlation features like `sqft_living` and `grade` using Seaborn heatmaps.
2.  **Data Cleaning:** Handled non-numeric date strings and identified multicollinearity.
3.  **Feature Engineering (The Smart Way):**
    * **House Age:** Calculated property age at the time of sale (`sold_year - yr_built`).
    * **Renovation Flag:** Created a binary feature (`is_renovated`) to give the model a clear signal on property upgrades.
4.  **Modeling:** Implemented **Multiple Linear Regression** using a 70/30 Train-Test split.

## 📈 Performance Results
After engineering the features, the model achieved the following metrics:
* **R² Score:** `0.6453` (Explaining ~65% of price variance).
* **Mean Absolute Error (MAE):** Check your notebook for the exact dollar amount!
* **Key Predictor:** `sqft_living` and `grade` proved to be the strongest influencers on price.

## 🧰 Tech Stack
* **Language:** Python 3
* **Libraries:** Pandas, NumPy, Scikit-Learn
* **Visuals:** Matplotlib, Seaborn
* **Environment:** Google Colab / Jupyter Notebook

## 🚀 How to Run
1.  Clone this repository.
2.  Open the `.ipynb` file in Google Colab or Jupyter.
3.  Ensure you have the latest versions of `scikit-learn` and `pandas` installed.

## 🔮 Future Work
* Implement **Random Forest** or **XGBoost** to capture non-linear relationships.
* Deploy the model as a live web application using **Streamlit**.
