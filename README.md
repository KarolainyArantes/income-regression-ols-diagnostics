# Income Regression — OLS Diagnostics and Model Specification

## 📌 Overview
This project documents an applied study of income modeling using **Ordinary Least Squares (OLS)**, with emphasis on **model specification, residual diagnostics, and assumption validation**.

Rather than focusing only on prediction, the goal is to understand how regression assumptions behave in practice and how transformations and additional variables **improve model consistency and interpretability**.

---

## 🎯 Objectives
- Build an income regression model using OLS
- Diagnose violations of OLS assumptions
- Apply log transformation to correct skewness
- Improve model specification with additional explanatory variables
- Perform professional residual analysis

---

## 🧰 Tools & Libraries
- Python
- Pandas
- Patsy
- Statsmodels
- Seaborn
- Matplotlib

---

## 🗂️ Model Specification

Initial model:

```python
renda ~ tempo_emprego
```
Improved model:
```python
log(renda) ~ tempo_emprego + sexo + posse_de_imovel + idade
```


---

## 🔍 Diagnostic Analysis Performed

The project includes the three essential OLS diagnostic visualizations:

1. Residuals vs Explanatory Variable
2. Residuals vs Fitted Values
3. QQ-Plot of Residuals

These plots are used to assess:

- Heteroscedasticity
- Model misspecification
- Normality of residuals
  
--- 

## ✅ Key Findings
- Income is highly skewed and requires log transformation
- Adding relevant variables significantly improves model behavior
- Residuals become approximately normal after transformation
- The model satisfies key OLS assumptions
- Even with moderate R², the model becomes statistically reliable and economically interpretable

--- 

## 📈 Lessons Learned

> A regression model is not validated by R² alone, but by how well it respects OLS assumptions and how well specified it is.


## 🚀 Conclusion

This repository demonstrates a practical journey from a poorly specified linear model to a statistically consistent log-linear model through proper diagnostics, transformation, and specification improvements.
