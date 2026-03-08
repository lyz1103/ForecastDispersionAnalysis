# Stock Dispersion Analysis: Analyst Disagreement and Market Volatility

## Project Overview
This project investigates whether **analyst disagreement about company fundamentals** is related to **future stock volatility**. When analysts produce very different forecasts for the same company, it may signal uncertainty or hidden information in the market.

The analysis measures **dispersion in analyst revenue forecasts** and evaluates whether this disagreement can help explain or predict stock price movements.

The project combines **statistical analysis, regression modeling, and machine learning** to study the relationship between analyst disagreement and stock volatility.

---

## Research Question

Does greater disagreement among financial analysts lead to **higher stock volatility**?

Specifically:

- When analysts strongly disagree about revenue forecasts, does the stock experience larger price movements?
- Can dispersion metrics provide predictive information about market risk?

---

## Methodology

### Data Preparation
- Collect analyst revenue forecasts and stock price data
- Compute dispersion metrics such as **coefficient of variation (CV)** of analyst estimates
- Apply transformations to stabilize variables

### Feature Engineering
Key features include:

- Revenue forecast dispersion
- Distribution shape metrics
- Analyst coverage counts
- Statistical characteristics of forecast distributions

### Modeling

Two modeling approaches are used:

**Linear Models**
- Linear regression to test the basic relationship between analyst dispersion and stock volatility

**Nonlinear Models**
- Decision tree / random forest models to capture nonlinear relationships

Results suggest nonlinear models slightly outperform linear models, indicating the relationship between analyst disagreement and volatility is complex.

---

## Additional Analysis

### High Analyst Coverage Subsample

To reduce noise from thinly covered firms, the analysis is repeated using only companies with **high analyst coverage**.

Findings show that dispersion metrics become more informative when analyst forecasts are more reliable.

### Hypothesis Testing

Stocks are grouped by dispersion level:

- Top 20% of dispersion (high analyst disagreement)
- Bottom 20% of dispersion (low disagreement)

This comparison helps isolate whether disagreement is associated with **greater stock price movement**.

---

## Key Findings

- Analyst disagreement has a measurable relationship with stock volatility.
- The relationship appears **nonlinear and complex**.
- Dispersion metrics are more predictive when analyst coverage is high.
- Forecast disagreement may serve as a **signal of market uncertainty**.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Data visualization libraries

---

## Possible Extensions

Future improvements could include:

- Incorporating additional firm-level and macroeconomic variables
- Testing trading strategies based on analyst dispersion signals
- Applying more advanced machine learning models
- Expanding the dataset across longer time periods

---

## Motivation

Understanding analyst disagreement helps quantify **information uncertainty in financial markets**. Dispersion-based signals are widely studied in quantitative finance and may help investors better assess risk and volatility.
