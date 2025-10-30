# STAT 601 – Week 8 Project

This repository contains my R Markdown (`.Rmd`) and rendered PDF file for Week 8 of STAT 601: Modern Applied Statistics I.  
The assignment focuses on **Simple Linear Regression (SLR)**, assumption testing, model comparison, and diagnostic evaluation of regression models for two drugs (A and G).

##  Contents
- **Julius Hai STAT 601 Project 8. Rmd** – R Markdown source file containing model setup, regression fitting, diagnostics, and interpretations.  
- **Julius Hai STAT 601 Project 8.pdf** – Rendered PDF output with complete solutions, plots, and conclusions.

## 🧠 Topics Covered

### 1️⃣ Simple Linear Regression Model
The **Simple Linear Regression (SLR)** model explains the relationship between a dependent variable \( Y \) and an independent variable \( X \) through a linear function:  
\[
Y_i = \beta_0 + \beta_1 X_i + \varepsilon_i
\]
where:
- \( \beta_0 \) = intercept,  
- \( \beta_1 \) = slope (rate of change),  
- \( \varepsilon_i \) = random error term.  

In this analysis, regression models were fitted separately for **Drug A** and **Drug G** to examine how dose level affects half-life.

---

### 2️⃣ Model Assumptions
The classical SLR model relies on four key assumptions:
1. **Linearity** – The relationship between \( X \) and \( Y \) is linear.  
2. **Independence** – Observations are independent of one another.  
3. **Homoscedasticity** – Variance of errors is constant across all values of \( X \).  
4. **Normality** – The residuals are normally distributed.  

These assumptions were verified using residual plots, QQ plots, and the Shapiro–Wilk test.

---

### 3️⃣ Model Fitting and ANOVA
Regression coefficients for **Drug A** and **Drug G** were estimated using R.  
The ANOVA tables (`anova(model)`) were compared side-by-side to assess the significance of slope coefficients.

- **Hypotheses:**  
  - \( H_0: \beta_1 = 0 \) → No linear relationship between dose and half-life.  
  - \( H_a: \beta_1 \neq 0 \) → A linear relationship exists.  

Decision rules were based on **p-values (α = 0.05)** to determine whether to reject \( H_0 \).

---

### 4️⃣ Scatterplots and Regression Lines
Fitted regression lines were plotted with scatterplots for both drugs:  
- **Drug G (red)** showed a strong positive slope — higher doses increase half-life.  
- **Drug A (blue)** displayed a weak negative slope — suggesting an opposite trend.  

The lines are **not parallel**, indicating that the two drugs have distinctly different dose-response behaviors, which is crucial for determining safe and effective dosing strategies.

---

### 5️⃣ Normality Diagnostics
The **QQ plots** and **Shapiro–Wilk tests** were performed for both models to evaluate residual normality.

- **Null hypothesis (H₀):** Residuals are normally distributed.  
- **Decision rule:** Reject H₀ if *p < 0.05*.  

Both visual (QQ plot) and numerical (Shapiro–Wilk) results guided the interpretation of model validity and fit quality.

---

### 6️⃣ Model Comparison and Interpretation
Manual calculations (based on examples from pages 340–341) were performed to validate regression estimates for each model.  
The fit of each model was then evaluated in terms of explanatory strength (R²), slope direction, and practical interpretation of how **dose level influences half-life**.

---

##  Author
**Julius Hai**  
Graduate Student – South Dakota State University

