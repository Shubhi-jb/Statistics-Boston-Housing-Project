# 📈 Statistics for Data Science: Boston Housing Project

This repository contains a comprehensive statistical analysis of the **Boston Housing Dataset**. The project explores the relationships between home values and various social, economic, and environmental factors using Python-based data science tools.

---

## 📊 Project Overview

The analysis follows a structured data science workflow divided into three key phases:

1. **Exploratory Data Analysis (EDA):** Initial data inspection, checking for missing values, and identifying data types.
2. **Data Visualization:** Using graphical methods to identify trends and distributions.
3. **Hypothesis Testing:** Applying formal statistical methods to validate assumptions about the data.

---

## 🔍 Key Statistical Findings

### 1. Impact of Distance on Home Values

An **Ordinary Least Squares (OLS) Regression** was performed to evaluate the impact of weighted distances to five Boston employment centres (`DIS`) on the median value of homes (`MEDV`).

- **Result:** The p-value was `0.000`, significantly below the `0.05` threshold.
- **Conclusion:** We reject the null hypothesis. There is a statistically significant relationship where home values increase by approximately **1.09 units** for every additional unit of distance from employment centres. However, the R² of `0.062` indicates that distance alone explains only 6.2% of the variation in home prices — other factors also play a significant role.

---

### 2. Environmental Factors & Industry

A **Pearson Correlation** test was conducted to assess the relationship between nitric oxide concentrations (`NOX`) and the proportion of non-retail business acres per town (`INDUS`).

- **Result:** A strong positive correlation of **0.76** was found.
- **Conclusion:** Higher industrial activity in a town is strongly associated with higher levels of air pollution.

---

### 3. Influence of the Charles River

A **T-test for Independent Samples** was used to determine whether houses near the Charles River (`CHAS`) had different median values than those further away. Levene's test (p=0.033) confirmed unequal variances between the two groups, so the test was run accordingly.

- **Result:** The p-value was `0.0036`, below the `0.05` threshold.
- **Conclusion:** There is a significant difference; homes near the river tend to have **higher median values**.

---

### 4. Age of Housing Stock & Home Values

A one-way **ANOVA test** was conducted to compare median home values (`MEDV`) across three age groups based on the proportion of units built before 1940 (`AGE`): 35 years and younger, between 35 and 70 years, and 70 years and older.

- **Result:** The p-value was effectively `0` ($1.71 \times 10^{-15}$).
- **Conclusion:** There is a statistically significant difference in median home values across age groups. Newer neighbourhoods tend to command higher property values.

---

## 🛠️ Technologies Used

| Tool | Purpose |
|------|---------|
| **Python 3** | Core programming language |
| **Pandas** | Data structure and manipulation |
| **Matplotlib & Seaborn** | High-quality data visualizations |
| **Scipy & Statsmodels** | T-tests, ANOVA, and OLS Regression |

---

## 📂 Repository Structure

```
├── Statistics_Project.ipynb   # Main Jupyter Notebook with code, visualizations & interpretations
└── README.md                  # Project documentation and summary of findings
```
