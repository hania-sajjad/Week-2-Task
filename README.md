# Week-2-Task
Deep Exploratory Analysis, Feature Engineering & Baseline Modeling

# Steel Industry Energy Consumption Analysis & Baseline Regression Models

## Project Overview

This project analyzes the **Steel Industry Energy Consumption Dataset** from the UCI Machine Learning Repository. The objective is to perform comprehensive exploratory data analysis (EDA), engineer meaningful features, and build baseline machine learning regression models to predict energy consumption.

The project follows a real-world machine learning workflow, beginning with data exploration and preprocessing, followed by model development, evaluation, and selection.

---

## Dataset

* **Dataset:** Steel Industry Energy Consumption Dataset
* **Source:** UCI Machine Learning Repository
* **Link:** https://archive.ics.uci.edu/static/public/851/steel+industry+energy+consumption.zip
* **Target Variable:** `Usage_kWh`

The dataset contains real-world electricity consumption records collected from a steel manufacturing plant, including power factors, reactive power, load types, timestamps, and operational information.

---

## Project Structure

```text
Week2-Steel-Energy/
│
├── week2_eda.ipynb
├── week2_baseline_models.ipynb
├── README.md
├── requirements.txt
│
└── data/
    ├── Steel_industry_data.csv
    └── steel_energy_engineered.csv
```

---

## Part 1 – Exploratory Data Analysis & Feature Engineering

The first notebook includes:

* Dataset loading and inspection
* Missing value analysis
* Data type verification
* Datetime conversion and feature extraction
* Creation of new engineered features:

  * Hour
  * Month
  * Day Name
  * Day Type (Weekday/Weekend)
  * Power Factor Ratio
  * High Load Indicator
* Outlier detection using the IQR method
* Correlation analysis using a heatmap
* Energy consumption analysis by load type
* Hourly energy consumption visualization
* EDA summary and observations

---

## Part 2 – Baseline Regression Modeling

The second notebook includes:

* Loading the engineered dataset
* Data preprocessing
* One-hot encoding of categorical variables
* Train-test split (80:20)
* Training four regression models:

  * Linear Regression
  * Ridge Regression
  * Decision Tree Regressor
  * Random Forest Regressor
* Model evaluation using:

  * Mean Absolute Error (MAE)
  * Root Mean Squared Error (RMSE)
  * R² Score
* 5-Fold Cross-Validation
* RMSE comparison visualization
* Predicted vs Actual scatter plot
* Model selection based on evaluation metrics

---

## Results Summary

| Model                       | Performance                   |
| --------------------------- | ----------------------------- |
| Linear Regression           | Good baseline performance     |
| Ridge Regression            | Similar to Linear Regression  |
| Decision Tree Regressor     | Excellent predictive accuracy |
| **Random Forest Regressor** | **Best overall performance**  |

The Random Forest Regressor achieved the lowest prediction error and the highest coefficient of determination (R²), making it the selected baseline model for this project.

---

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## How to Run

1. Download or clone this repository.
2. Open the notebooks in Google Colab or Jupyter Notebook.
3. Install the required libraries:

```bash
pip install -r requirements.txt
```

4. Run the notebooks in the following order:
   - `week2_eda.ipynb`
   - `week2_baseline_models.ipynb`

---

## Author

**Hania Sajjad**

AI/ML Internship Task – Week 2
