# 📊 HR Employee Attrition Prediction

## Executive Summary
Employee attrition (turnover) is a major cost to organizations, impacting productivity, morale, and recruitment budgets. This project utilizes machine learning—specifically **Logistic Regression**—to analyze a dataset of HR records. 

The goal is two-fold:
1. **Business Inference:** Identify the statistically significant drivers behind *why* employees leave.
2. **Predictive Modeling:** Build a classification model to proactively flag high-risk employees so Human Resources can implement targeted retention strategies.

---

## 💡 Key Business Insights
By converting the model's log-odds into actionable **Odds Ratios**, this analysis uncovered several critical retention drivers:

* **Commute Fatigue (Geographical):** Distance from home is a statistically proven driver of turnover. For every 1 additional mile added to an employee's commute, their odds of quitting increase by roughly **4%**.
* **Satisfaction Matters (Behavioral):** For every 1-point increase in an employee's job satisfaction rating, their odds of leaving the company drop by **27%**.
* **Early-Career Flight Risk (Demographic):** For every additional year of age, the odds of attrition decrease by **4%**. Furthermore, single employees represent a significantly higher flight risk compared to married peers, indicating a need for localized, early-career retention strategies.

---

## ⚙️ Methodology & Tech Stack
* **Language:** R
* **Libraries:** `ggplot2`, `stats` (base R)
* **Techniques Used:**
  * Exploratory Data Analysis (EDA)
  * Feature Engineering
  * Data Preprocessing (Removing zero-variance predictors)
  * Train/Test Split (70/30)
  * Logistic Regression (Binomial)
  * Odds Ratio Interpretation
  * Confusion Matrix Evaluation

---

## 📈 Model Performance
The Logistic Regression model successfully learned the underlying patterns of employee turnover. When tested against unseen data (the 30% holdout set), the model achieved an overall **Accuracy of 83.9%**, proving that employee attrition can be mathematically anticipated and intercepted.

---

## 📂 Repository Structure
* `HR-Employee-Attrition.csv`: The raw dataset containing 35 HR variables (Age, JobRole, MonthlyIncome, etc.).
* `Employee_Attrition.Rmd`: The raw R Markdown script containing all code, mathematical transformations, and visualizations.
* `Employee_Attrition.html`: The fully compiled, interactive HTML report designed for non-technical stakeholders.

---

## 🚀 How to View This Project

### Option 1: View the Live Report (Recommended)
You can view the fully formatted, interactive HTML report directly in your browser without needing to download any software.
*(Note: Insert your live GitHub Pages link here once activated!)*

### Option 2: Reproduce the Code
To run this project locally:
1. Clone this repository to your local machine.
2. Ensure both the `.csv` file and the `.Rmd` file are in the same working directory.
3. Open `Employee_Attrition.Rmd` in RStudio.
4. Click the **Knit** button to install any missing packages and generate the HTML report.
