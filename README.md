# Walmart Sales: Advanced Statistical Analysis & Hypothesis Testing

---

**Course:** Advanced Applied Statistics
**Dataset:** Walmart Weekly Sales
**Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/mikhail1681/walmart-sales)
**Environment:** VS Code & Virtual Environment (`venv`)
**Version Control:** Git

---

## Project Overview

This project performs a comprehensive statistical evaluation of Walmart's weekly sales data across 45 stores (6,435 records). The primary goal is to rigorously implement and interpret a wide range of statistical tests, ensuring all assumptions are verified and results are properly contextualized.

## Project Structure

| Folder | Description |
|--------|-------------|
| `data/` | Raw dataset (`Walmart_Sales.csv`) |
| `notebooks/` | Analysis notebook |

## Dataset Description

| Column | Description |
|--------|-------------|
| `Store` | Store identifier (1–45) |
| `Date` | Week of sales record |
| `Weekly_Sales` | Total sales for the store that week |
| `Holiday_Flag` | 1 if the week includes a holiday, 0 otherwise |
| `Temperature` | Average regional temperature |
| `Fuel_Price` | Regional fuel price |
| `CPI` | Consumer Price Index |
| `Unemployment` | Regional unemployment rate |

## Statistical Tests Roadmap

1. **Z-Test:** One-sample & two-sample Z-tests for means
2. **T-Test:** One-sample, independent (with Levene's test for equal variance), and paired T-tests
3. **U-Test (Mann-Whitney):** Non-parametric alternative for independent groups
4. **ANOVA:** One-way & two-way ANOVA (with Tukey HSD post-hoc)
5. **Chi-Square Test:** Test of independence between categorical variables
6. **A/B Testing:** Full statistical framework for business decision-making (power analysis, MDE, Welch's T-test)
7. **Distribution & Normality Testing:** Skewness, kurtosis, and Kolmogorov-Smirnov test

## Sections

1. Data Loading & Initial Exploration
2. Data Preprocessing & Feature Engineering
3. Z-Test (One-Sample & Two-Sample)
4. T-Test (One-Sample, Independent, and Paired)
5. Mann-Whitney U-Test (Non-parametric Test)
6. Analysis of Variance (ANOVA)
7. Chi-Square Test of Independence
8. Business A/B Testing Framework
9. Distribution Analysis & Normality Testing

## Setup & Installation

Clone the repository and set up a virtual environment:

    git clone https://github.com/Arian11z/data-analysis-projects.git
    cd data-analysis-projects/walmart-statistical-analysis

    python -m venv venv
    venv\Scripts\activate        # Windows
    source venv/bin/activate     # macOS/Linux

    pip install -r requirements.txt

## Usage

Launch Jupyter and open the notebook:

    jupyter notebook notebooks/walmart_statistical_analysis.ipynb

## Tools & Libraries

- Python 3.11
- pandas, numpy
- matplotlib, seaborn
- scipy
- statsmodels

## Key Findings

- Weekly sales show a statistically significant difference between holiday and non-holiday weeks.
- Sales distributions across stores are non-normal, motivating both parametric and non-parametric test comparisons.
- Year and holiday status jointly influence weekly sales (two-way ANOVA interaction effect).
- Regional unemployment level is associated with a measurable shift in average weekly sales, informing the A/B testing framework for promotional budget decisions.

---

*Part of the [data-analysis-projects](https://github.com/Arian11z/data-analysis-projects) portfolio.*
