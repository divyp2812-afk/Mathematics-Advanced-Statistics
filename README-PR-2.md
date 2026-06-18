# Statistical Analysis and Hypothesis Testing Using Python

## Project Overview

This project demonstrates the application of **Inferential Statistics** and **Hypothesis Testing** using Python. The analysis is performed on a healthcare dataset to understand relationships between variables and validate statistical assumptions using various hypothesis tests.

The project is divided into two parts:

- **Part A:** Theoretical concepts of Inferential Statistics and Hypothesis Testing.
- **Part B:** Practical implementation of statistical techniques using Python.

---

## Objectives

- Understand Inferential Statistics concepts.
- Learn the process of Hypothesis Testing.
- Calculate Confidence Intervals.
- Perform T-Test, Chi-Square Test, and ANOVA.
- Analyze relationships using Covariance and Correlation.
- Interpret statistical results effectively.

---

##  Dataset

**Dataset File:** `health_dataset.csv`

The dataset contains healthcare-related information such as:

- Age
- Gender
- Weight
- BMI
- Smoking Status
- Diabetes Status

---

## Technologies Used

- Python 3.x
- Jupyter Notebook
- Pandas
- NumPy
- SciPy

### Install Required Libraries

```bash
pip install pandas numpy scipy
```

---

# Part A: Inferential Statistics & Hypothesis Testing

## What is Inferential Statistics?

Inferential Statistics is the branch of statistics that uses sample data to make predictions or draw conclusions about a population.

### Applications

- Population estimation
- Decision making
- Prediction and forecasting
- Hypothesis testing

---

## What is Hypothesis Testing?

Hypothesis Testing is a statistical method used to determine whether there is enough evidence in a sample dataset to support a specific claim about a population.

### Key Terms

### Null Hypothesis (H₀)

Assumes no significant difference or relationship exists.

### Alternative Hypothesis (H₁)

Assumes a significant difference or relationship exists.

### Significance Level (α)

The probability threshold used to determine statistical significance (commonly 0.05).

### P-value

The probability of obtaining results as extreme as those observed if the null hypothesis is true.

### Decision Rule

- If p-value < 0.05 → Reject H₀
- If p-value ≥ 0.05 → Fail to Reject H₀

---

# Part B: Statistical Analysis Using Python

## 1. Hypothesis Formulation

### Hypothesis 1

**H₀:** Smoking status and diabetes are independent.

**H₁:** Smoking status and diabetes are associated.

### Hypothesis 2

**H₀:** Mean BMI is equal across groups.

**H₁:** Mean BMI differs across groups.

---

## 2. Confidence Interval Calculation

The notebook calculates 95% Confidence Intervals for:

- Age
- Weight
- BMI

These intervals estimate the range within which the true population mean is expected to lie.

---

## 3. Independent T-Test

### Objective

Compare BMI values between Male and Female participants.

### Interpretation

- p-value < 0.05 → Significant difference exists.
- p-value ≥ 0.05 → No significant difference exists.

---

## 4. Chi-Square Test

### Objective

Determine whether Smoking Status and Diabetes Status are associated.

### Example

```python
pd.crosstab(df['smoking_status'], df['diabetes'])
```

### Interpretation

- p-value < 0.05 → Variables are associated.
- p-value ≥ 0.05 → Variables are independent.

---

## 5. ANOVA Test

### Objective

Compare BMI across multiple age groups.

### Age Categories

- Young
- Middle Age
- Senior
- Old

### Interpretation

- p-value < 0.05 → At least one group mean differs.
- p-value ≥ 0.05 → No significant difference among groups.

---

## 6. Covariance Analysis

Covariance measures how two variables change together.

In this project:

- Age and BMI covariance is calculated.
- Positive covariance indicates variables move together.
- Negative covariance indicates inverse movement.

---

## 7. Correlation Analysis

Correlation measures the strength and direction of a relationship between variables.

### Correlation Scale

| Correlation Value | Interpretation |
|------------------|---------------|
| +1 | Perfect Positive Correlation |
| 0 | No Correlation |
| -1 | Perfect Negative Correlation |

---

## Results

The project successfully demonstrates:

- Confidence Interval Estimation
- Independent T-Test
- Chi-Square Test
- ANOVA Test
- Covariance Calculation
- Correlation Analysis

---

## Learning Outcomes

After completing this project, you will be able to:

- Apply inferential statistics concepts.
- Formulate null and alternative hypotheses.
- Perform statistical tests using Python.
- Interpret p-values and confidence intervals.
- Analyze relationships between variables.
- Make data-driven decisions.

---

## How to Run

1. Download the project files.
2. Install required libraries.

```bash
pip install pandas numpy scipy
```

3. Open Jupyter Notebook.

```bash
jupyter notebook
```

4. Run all cells in:

- PART-A.ipynb
- PART-B.ipynb

---
