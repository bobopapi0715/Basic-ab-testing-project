# Basic-ab-testing-project
A/B testing analysis on landing page conversion
# 📊 Basic A/B Testing Project – Landing Page Conversion

This project analyzes the results of an A/B test conducted by an e-commerce company to evaluate whether a new landing page improves conversion rates compared to the existing version.

---

## 🎯 Objectives

- Assess if the new page (Version B) performs significantly better than the original (Version A)
- Perform hypothesis testing (two-proportion z-test)
- Provide business insight based on statistical evidence

---

## 📁 Dataset

- **Source**: [Kaggle - A/B Testing Dataset](https://www.kaggle.com/datasets/amirmotefaker/ab-testing-dataset)
- File used: `ab_data.csv`
- The dataset includes user visits, group assignment (control/treatment), and whether they converted

---

## 🛠️ Tools & Techniques

- Python (`pandas`, `scipy`, `statsmodels`)
- Jupyter Notebook
- Exploratory Data Analysis (EDA)
- Hypothesis Testing (z-test for proportions)
- Data Cleaning & Validation

---

## 📈 Key Results

- Conversion Rate A (control): **~12.1%**
- Conversion Rate B (treatment): **~12.9%**
- **p-value**: > 0.05 → No statistically significant difference
- Recommendation: Do not launch new page without further testing or segmentation

---

## 📌 Business Impact

- Demonstrates how data-driven decision making can avoid unnecessary rollout
- Highlights the importance of statistical rigor in A/B testing
- Suggests follow-up actions such as:
  - Testing with larger sample size
  - Segmenting users by geography or device type

---

## ✅ Files in This Repository

| File | Description |
|------|-------------|
| `ab_testing_analysis.ipynb` | Main analysis notebook |
| `README.md` | This file |
| `ab_data.csv` (optional) | Dataset if allowed, or linked to source |

---

## 💡 Next Steps (Optional Ideas)

- Perform segmentation-based A/B tests
- Visualize conversion funnel drop-off
- Build a Streamlit dashboard to interact with the test results

---

## 🙋‍♀️ About Me

Hi! I’m Yingyi Li — a data & analytics enthusiast with a background in statistics (UCSD) and applied data science (USC). I’m exploring how statistical inference and machine learning can be used to drive better business decisions.

📫 Connect: [LinkedIn](https://www.linkedin.com/in/YOUR-LINK) | 📧 papilee0715@gmail.com
