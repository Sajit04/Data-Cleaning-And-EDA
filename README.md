# Data-Cleaning-And-EDA
# Part 1 - Exploratory Data Analysis (EDA) & Data Cleaning

## Overview

In this part, I performed Exploratory Data Analysis (EDA) and data preprocessing on the **Adult Income Dataset**. The objective was to understand the dataset, identify missing values, detect outliers, analyze feature relationships, and prepare a clean dataset for machine learning.

## Dataset

- **Dataset:** Adult Income Dataset
- **Input File:** `adult.csv`
- **Output File:** `cleaned_data.csv`

### Why this dataset?

I selected the Adult Income Dataset because it contains both numerical and categorical features and is widely used for classification tasks. It is suitable for practicing data cleaning, visualization, and machine learning.

---

## Data Cleaning

The following preprocessing steps were performed:

- Removed duplicate records
- Handled missing values using appropriate imputation methods
- Encoded categorical variables
- Detected and handled outliers using the IQR method
- Saved the cleaned dataset as `cleaned_data.csv`

After preprocessing:

```python
df.isnull().sum()
```

confirmed that **no missing values remained** in the dataset.

---

## Statistical Analysis

The **mean** and **median** were calculated for the two most skewed numerical columns.

- For positively skewed data, the **median** is a better measure of central tendency because it is less affected by extreme values.
- For approximately symmetric data, the **mean** provides a good representation of the center of the distribution.

---

## Visualizations

The following visualizations were created:

- Histogram
- Scatter Plot
- Box Plot
- Correlation Heatmap

### Scatter Plot Interpretation

The scatter plot was used to observe relationships between numerical variables. It showed the distribution of data points and helped identify possible trends and outliers.

### Box Plot Interpretation

The box plot was used to detect outliers using the interquartile range (IQR). Extreme values outside the whiskers were identified and analyzed.

### Heatmap Interpretation

The heatmap displayed the correlation between numerical features. Strong positive or negative correlations indicate variables that may influence each other.

**Alternative Explanation:** A high correlation does not necessarily imply causation. Two variables may appear strongly related due to the influence of other factors.

---

## IQR Analysis

Outliers were identified using the Interquartile Range (IQR) method.

- **Analysis 1:** The first selected numerical feature contained several outliers above the upper bound, indicating a right-skewed distribution.
- **Analysis 2:** The second selected numerical feature showed fewer outliers, suggesting a more balanced distribution.

---

## Files

```
Part1_EDA.ipynb
adult.csv
cleaned_data.csv
README.md
```

---

## Conclusion

This part focused on understanding and cleaning the Adult Income Dataset. After handling missing values, outliers, and feature analysis, a clean dataset was prepared for use in the machine learning tasks of Part 2.
