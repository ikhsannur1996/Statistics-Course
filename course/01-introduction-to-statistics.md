# Chapter 01 — Introduction to Statistics

## Learning Objectives

By the end of this chapter, you will be able to:

- Explain what statistics is and why it matters.
- Distinguish between descriptive statistics and inferential statistics.
- Identify populations, samples, variables, and observations.
- Classify common data types.
- Use Python, NumPy, Pandas, and Matplotlib for basic statistical analysis.

---

## 1. What Is Statistics?

Statistics is the science of collecting, organizing, analyzing, interpreting, and presenting data.

Statistics helps us answer practical questions such as:

- What is the average monthly income of customers?
- Which product category performs best?
- Is a new marketing campaign better than the old one?
- Can we estimate a population value using only a sample?

In data science and business intelligence, statistics helps transform raw data into useful insight.

---

## 2. Why Statistics Matters

Raw data is often too large or too complex to understand directly. Statistics helps summarize data, detect patterns, measure uncertainty, and support decision-making.

For example, instead of reading thousands of customer records one by one, we can calculate:

- Average income
- Median age
- Total revenue
- Standard deviation
- Customer growth rate
- Transaction frequency

These summaries make data easier to understand.

---

## 3. Descriptive Statistics

Descriptive statistics focuses on summarizing and describing data.

Common descriptive statistics include:

| Measure | Description |
|---|---|
| Mean | Average value |
| Median | Middle value |
| Mode | Most frequent value |
| Minimum | Smallest value |
| Maximum | Largest value |
| Range | Maximum minus minimum |
| Variance | Average squared distance from the mean |
| Standard deviation | Typical distance from the mean |

### Example

Suppose we have the following scores:

```text
70, 75, 80, 85, 90
```

The mean is:

```text
(70 + 75 + 80 + 85 + 90) / 5 = 80
```

So, the average score is `80`.

---

## 4. Inferential Statistics

Inferential statistics uses sample data to make conclusions about a larger population.

It helps answer questions such as:

- Is a new product significantly better than the old product?
- What is the estimated average income of all customers?
- Is there a relationship between education level and salary?
- Can we predict future sales using historical data?

Inferential statistics is useful because collecting data from an entire population is often expensive, slow, or impossible.

---

## 5. Population and Sample

A **population** is the complete group we want to study.

A **sample** is a smaller group selected from the population.

Example:

```text
Population = All bank customers
Sample = 1,000 selected bank customers
```

The goal is to use the sample to understand the population.

---

## 6. Variables and Observations

In a dataset:

- An **observation** is one row or record.
- A **variable** is one column or feature.

Example:

| Customer ID | Age | Income | Account Type |
|---|---:|---:|---|
| C001 | 25 | 7000000 | Savings |
| C002 | 31 | 12000000 | Current |
| C003 | 40 | 15000000 | Savings |

In this dataset:

- Each customer is an observation.
- Age, income, and account type are variables.

---

## 7. Types of Data

Data can be classified into numerical and categorical data.

### Numerical Data

Numerical data represents numbers.

It can be divided into:

1. **Discrete data** — countable values, such as number of customers.
2. **Continuous data** — values measured on a scale, such as weight, income, or temperature.

### Categorical Data

Categorical data represents labels or groups.

It can be divided into:

1. **Nominal data** — categories with no order, such as city or product type.
2. **Ordinal data** — categories with order, such as low, medium, and high.

---

## 8. Mathematical Notation

Common statistical symbols:

| Symbol | Meaning |
|---|---|
| `n` | Sample size |
| `N` | Population size |
| `x` | Individual data value |
| `x̄` | Sample mean |
| `μ` | Population mean |
| `s` | Sample standard deviation |
| `σ` | Population standard deviation |

The sample mean is calculated as:

```text
x̄ = (x₁ + x₂ + ... + xₙ) / n
```

Example:

```text
Data = 10, 20, 30, 40, 50
x̄ = (10 + 20 + 30 + 40 + 50) / 5
x̄ = 30
```

---

## 9. Python Example

```python
scores = [70, 75, 80, 85, 90]

mean_score = sum(scores) / len(scores)

print(mean_score)
```

Expected output:

```text
80.0
```

---

## 10. NumPy Example

```python
import numpy as np

scores = np.array([70, 75, 80, 85, 90])

print("Mean:", np.mean(scores))
print("Median:", np.median(scores))
print("Minimum:", np.min(scores))
print("Maximum:", np.max(scores))
print("Standard Deviation:", np.std(scores))
```

Expected output:

```text
Mean: 80.0
Median: 80.0
Minimum: 70
Maximum: 90
Standard Deviation: 7.0710678118654755
```

---

## 11. Pandas Example

```python
import pandas as pd

data = {
    "customer_id": ["C001", "C002", "C003", "C004", "C005"],
    "age": [25, 31, 40, 35, 28],
    "income": [7000000, 12000000, 15000000, 10000000, 8500000],
    "account_type": ["Savings", "Current", "Savings", "Savings", "Current"]
}

df = pd.DataFrame(data)

print(df)
print(df.describe())
```

The `describe()` function produces a statistical summary of numerical columns.

---

## 12. Visualization Example

```python
import matplotlib.pyplot as plt

ages = [25, 31, 40, 35, 28]

plt.hist(ages, bins=5)
plt.title("Distribution of Customer Ages")
plt.xlabel("Age")
plt.ylabel("Frequency")
plt.show()
```

Image placeholder:

```markdown
![Distribution of Customer Ages](../assets/chapter-01-age-distribution.png)
```

---

## 13. Exercises

### Exercise 1

Define statistics in your own words.

### Exercise 2

Classify the following variables as numerical or categorical:

| Variable | Type |
|---|---|
| Age |  |
| City |  |
| Monthly income |  |
| Customer satisfaction level |  |
| Number of transactions |  |

### Exercise 3

Calculate the mean of the following data manually:

```text
5, 10, 15, 20, 25
```

### Exercise 4

Create a Python list containing the following values and calculate the mean:

```text
12, 18, 24, 30, 36
```

### Exercise 5

Create a Pandas DataFrame with the following columns:

- `student_name`
- `score`
- `grade`

Use at least five rows of data and summarize the numerical column using `describe()`.

---

## 14. Quiz

### Question 1

What is the main purpose of descriptive statistics?

A. To make predictions about future data  
B. To summarize and describe data  
C. To build machine learning models  
D. To collect data from the internet  

### Question 2

Which of the following is categorical data?

A. Age  
B. Salary  
C. City  
D. Temperature  

### Question 3

What is a sample?

A. The entire group being studied  
B. A smaller group selected from the population  
C. A mathematical formula  
D. A visualization method  

### Question 4

Which Python library is commonly used for tabular data?

A. NumPy  
B. Pandas  
C. Matplotlib  
D. Math  

### Question 5

What does `n` usually represent in statistics?

A. Population mean  
B. Sample size  
C. Standard deviation  
D. Median  

---

## 15. Solutions

### Solution 1

Statistics is the science of collecting, organizing, analyzing, interpreting, and presenting data to support decision-making.

### Solution 2

| Variable | Type |
|---|---|
| Age | Numerical |
| City | Categorical |
| Monthly income | Numerical |
| Customer satisfaction level | Categorical, ordinal |
| Number of transactions | Numerical, discrete |

### Solution 3

```text
Mean = (5 + 10 + 15 + 20 + 25) / 5
Mean = 75 / 5
Mean = 15
```

### Solution 4

```python
values = [12, 18, 24, 30, 36]
mean_value = sum(values) / len(values)
print(mean_value)
```

Expected output:

```text
24.0
```

### Solution 5

```python
import pandas as pd

data = {
    "student_name": ["Andi", "Budi", "Citra", "Dewi", "Eka"],
    "score": [80, 75, 90, 85, 70],
    "grade": ["B", "C", "A", "B", "C"]
}

df = pd.DataFrame(data)

print(df)
print(df.describe())
```

---

## 16. Quiz Answers

| Question | Answer |
|---|---|
| 1 | B |
| 2 | C |
| 3 | B |
| 4 | B |
| 5 | B |

---

## 17. Summary

In this chapter, you learned the meaning and purpose of statistics. You also learned the difference between descriptive and inferential statistics, the concepts of population and sample, and the difference between variables and observations.

You classified numerical and categorical data and used Python, NumPy, Pandas, and Matplotlib for basic statistical analysis.

---

## 18. References

- OpenIntro Statistics
- Think Stats by Allen B. Downey
- Practical Statistics for Data Scientists by Peter Bruce, Andrew Bruce, and Peter Gedeck
- Python Data Science Handbook by Jake VanderPlas
- NumPy Documentation
- Pandas Documentation
- Matplotlib Documentation
