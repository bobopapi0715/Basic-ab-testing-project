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
AB testing project 1/     # <-- Corrected name
├── control_group.csv     # <-- Raw data likely in root
├── test_group.csv        # <-- Raw data likely in root
├── data/
│   └── ab_test_cleaned.csv # <-- Correct save location
├── venv/                   # <-- Your virtual environment
├── .gitignore              # <-- Should exist
├── ab_test_analysis.ipynb  # <-- Correct notebook name, in root
├── README.md               # <-- This file
└── requirements.txt        # <-- Should exist

## Methodology
1.  **Data Cleaning & Preparation:** Loaded the data, checked for missing values, ensured correct data types.
2.  **Exploratory Data Analysis (EDA):** Calculated overall conversion rates and checked for any obvious issues or biases (e.g., Sample Ratio Mismatch).
3.  **Hypothesis Testing:**
    * Formulated null hypothesis ($H_0$) and alternative hypothesis ($H_a$).
    * Checked assumptions for the chosen statistical test.
    * Performed a [mention the specific statistical test, e.g., 'two-proportion z-test' or 'Chi-squared test'] to compare the conversion rates between Group A and Group B.
4.  **Conclusion:** Interpreted the p-value and confidence interval based on a pre-defined significance level (e.g., $\alpha = 0.05$) to make a decision on statistical significance.

## Key Findings
* **Control Group Conversion Rate (Purchases/Clicks):** 9.83% [cite: 1]
* **Treatment Group Conversion Rate (Purchases/Clicks):** 8.64% [cite: 1]
* **Calculated Z‑statistic:** 11.839 [cite: 1]
* **Calculated P‑value:** 0.0000 [cite: 1]
* **Conclusion:** Since the p-value (0.0000) is less than the significance level ($\alpha = 0.05$), the difference in conversion rates is **statistically significant**[cite: 1]. The results indicate the Control group performed significantly better than the Treatment group[cite: 1].
* **Recommendation:** **Do NOT roll out** the new landing page (version B). Continue using the original (Control) landing page design[cite: 1].

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
