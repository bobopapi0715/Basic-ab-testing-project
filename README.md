# 📊 A/B Testing: Landing Page Optimization

## Table of Contents
1.  [Project Summary](#project-summary)
2.  [Dataset](#dataset)
3.  [Repository Structure](#repository-structure)
4.  [Methodology](#methodology)
5.  [Key Findings](#key-findings)
6.  [Technologies Used](#technologies-used)
7.  [Setup and Usage](#setup-and-usage)
---

## Project Summary
This project analyzes the effectiveness of two landing page variants (control vs. treatment) in driving user conversions using data from Kaggle. We load session and purchase data, perform exploratory data analysis, check for statistical validity, visualize conversion rates, and run a two-proportion z-test to assess whether the new design (treatment group) yields a statistically significant uplift compared to the original (control group). The analysis includes data cleaning, hypothesis testing, and visualization, culminating in a recommendation based on the findings.

## Dataset
* **Source:** [Kaggle AB-testing dataset](https://www.kaggle.com/datasets/amirmotefaker/ab-testing-dataset)
* **Raw files Location:** `archive/` directory
    * `control_group.csv`
    * `test_group.csv`
* **Description:** The dataset contains user session/purchase information for two groups exposed to different landing page versions. Key columns include `user_id`, `group`, `landing_page`, and `converted`.

## Repository Structure
```bash
Basic-ab-testing-project/
├── archive/
│   ├── control_group.csv
│   └── test_group.csv
├── data/
│   └── ab_test_cleaned.csv       # cleaned & merged output
├── notebooks/
│   └── A_B_Testing_Landing_Page_Conversion.ipynb
├── tableau/
│   └── landing_page_dashboard.twbx   # interactive funnel dashboard
└── README.md

## Methodology
1.  **Data Cleaning & Preparation:** Loaded the data, checked for missing values, ensured correct data types.
2.  **Exploratory Data Analysis (EDA):** Calculated overall conversion rates and checked for any obvious issues or biases (e.g., Sample Ratio Mismatch).
3.  **Hypothesis Testing:**
    * Formulated null hypothesis ($H_0$) and alternative hypothesis ($H_a$).
    * Checked assumptions for the chosen statistical test.
    * Performed a [mention the specific statistical test, e.g., 'two-proportion z-test' or 'Chi-squared test'] to compare the conversion rates between Group A and Group B.
4.  **Conclusion:** Interpreted the p-value and confidence interval based on a pre-defined significance level (e.g., $\alpha = 0.05$) to make a decision on statistical significance.

## Key Findings
* **Control conversion rate:** 12.30%  
* **Treatment conversion rate:** 14.80%  
* **Z‑statistic:** 2.20  
* **P‑value:** 0.0283  
* At α = 0.05, the increase in conversion for version B is **statistically significant**.  
* **Recommendation:** Roll out version B, as it demonstrated a significant uplift.

## Technologies Used
* Python
* Pandas (for data manipulation)
* NumPy (for numerical operations)
* Statsmodels (for statistical testing)
* Matplotlib / Seaborn (for visualization)
* Jupyter Notebook (for analysis development)

## Setup and Usage

### 1. Clone the Repository
```bash
git clone [https://github.com/bobopapi0715/Basic-ab-testing-project.git](https://github.com/bobopapi0715/Basic-ab-testing-project.git)
cd Basic-ab-testing-project
