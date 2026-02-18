# Inequality, Economic Development and Interpersonal Trust (ESS 2023)

## Overview

This project investigates whether income inequality is associated with interpersonal trust in Europe, and to what extent economic development explains this relationship.

Using individual-level data from the European Social Survey (ESS Round 11, 2023) combined with macroeconomic indicators from Eurostat, the analysis examines how inequality and GDP per capita relate to generalized trust across European countries.

---

## Research Question

Is income inequality associated with interpersonal trust independently of economic development, or does economic development account for much of the observed relationship?

---

## Data Sources

- European Social Survey (ESS Round 11, 2023)
- Eurostat GDP per capita data
- Eurostat Gini coefficient data

Sample size: ~50,000 individual observations across European countries.

---

## Methodology

The analysis follows a structured empirical approach:

1. Individual-level regression analysis (OLS)
2. Country-level aggregation
3. Inclusion of GDP per capita as a development control
4. Robustness check using log(GDP per capita)

Standard linear regression models are estimated using `statsmodels` in Python.

---

## Project Structure

inequality-trust-europe/
│
├── data/
│ ├── raw/ # Original ESS and macro data
│ ├── processed/ # Cleaned and merged datasets
│
├── notebooks/
│ ├── 01_data_prep.ipynb # Data cleaning and merging
│ ├── 02_analysis.ipynb # Regression and visualization
│
├── results/
│ ├── figures/ # Generated plots
│ ├── tables/ # Regression outputs
│
├── requirements.txt
└── README.md


---

## Key Findings (Summary)

- Income inequality is negatively correlated with interpersonal trust.
- However, once GDP per capita is included, the inequality effect weakens.
- Economic development explains a significant portion of cross-country trust variation.

This suggests that structural economic conditions play a major role in shaping interpersonal trust levels.

---

## Reproducibility

To reproduce the analysis:

1. Clone the repository
2. Install dependencies:
   pip install -r requirements.txt
3. Run notebooks in order:
   - `01_data_prep.ipynb`
   - `02_analysis.ipynb`

---

## Tools Used

- Python
- pandas
- numpy
- statsmodels
- matplotlib
- seaborn

---

## Author

Independent research project by Atılgan Hacıeyüpoğlu.


