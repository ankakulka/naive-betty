---
title: "Exploratory Data Analysis"
weight: 1
bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
bookSearchExclude: false
type: "page"
---



# Exploratory Data Analysis

Learning Objectives:

 - Descriptive Statistics
 - GroupBy
 - ANOVA
 - Correlation
 - Correlation - Statistics

 ## Purpose of Exploratory Data Analysis

 - Explore data before building complicated models
 - Calculate descriptive statistics for your data
 - Describe basic fautures of data
 - Give short summaries 

Use `describe` method in Pandas:

 ```python
 datafram.describe()
 
 ```


Returns description of the data in the DataFrame. Output depends on the data provided. 

If the DataFrame contains **numerical data**, the description contains these information for each column:

count - The number of not-empty values.
mean - The average (mean) value.
std - The standard deviation.
min - the minimum value.
25% - The 25% percentile*.
50% - The 50% percentile*.
75% - The 75% percentile*.
max - the maximum value.

Example

```python
[5 rows x 29 columns]
        symboling  normalized-losses  ...      diesel         gas
count  201.000000          201.00000  ...  201.000000  201.000000
mean     0.840796          122.00000  ...    0.099502    0.900498
std      1.254802           31.99625  ...    0.300083    0.300083
min     -2.000000           65.00000  ...    0.000000    0.000000
25%      0.000000          101.00000  ...    0.000000    1.000000
50%      1.000000          122.00000  ...    0.000000    1.000000
75%      2.000000          137.00000  ...    0.000000    1.000000
max      3.000000          256.00000  ...    1.000000    1.000000

```

## Handling Categorical Data

Use Pandas `Value_Counts()` method. 

## Visualising Data

### Box Plots

Quartile ranges and outliers.

Example 
```python
sns.boxplot(x = "drive-wheels", y="price", data=df)

```

### Scatter Plots
Each point in a scatter plot represents an observation.
1. Predictor/independent variable on x-axis
2. Target/dependent variable on y-axis

Example in ython matplotlib (from matplotlib docs):

```python
import matplotlib.pyplot as plt
import numpy as np

# Fixing random state for reproducibility
np.random.seed(19680801)


N = 50
x = np.random.rand(N)
y = np.random.rand(N)
colors = np.random.rand(N)
area = (30 * np.random.rand(N))**2  # 0 to 15 point radii

plt.scatter(x, y, s=area, c=colors, alpha=0.5)
plt.show()

```

### Heatmap

Matplotlib

```python
import matplotlib as plt

plt.color(df_pivot, cmap="RdBu")
plt.colorbar()
plt.show()

```

## Grouping Data

Use Pandas `dataframe.groupBy()`method to:
- group data into categories
- apply to single or multiple variables
- apply to categoriacal variables

 ```python

 test_results = test.groupBy(['cat1, 'cat2], as_index= False).mean()
 
 ```

 `Pivot()` method in Pandas

 