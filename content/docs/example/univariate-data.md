---
title: "Univariate Data"
weight: 1
bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
bookSearchExclude: false
mermaid: true
---


# Univariate data

## Types of data

**Quantitative**  variables are  numerical, measurable quantities in which arithmetic operations often make sense.
These can be:
1. **Continuous**: could take on any possible value within an interval, many possible values.
    For example: height, weight, time
2. **Discrete**: countable value, finite number of values: has to take an integer value.
    For example: a number of children in a household

**Qualitative** (Categorical) variables classify individuals or items into different groups. 
1. **Ordinal**: groups that have an order or ranking
    For example: student ranking
2. **Nominal**: doesn't have any associates ranking with ranking with it.
    For example: marital status

## Qualitative (categorical) data 

pie chart or dot plot 
    - Comparison is easier on the dot plot
    - Pie chart is better at showing the percentage of the total that the category represents
    {{< expand "Problems with pie charts">}}  
    - Very small slices might overlap 
    - it is hard to compare slices without proper labeling: it is easier to compare when looking at a bar chart
    {{< /expand >}}


### Pie Chart, Bar Graph, Table







## Quantitative data

- **Quantitative**(numbers): bar chart and histogram
    - Bar chart: only the height of the bars is meaningful
    - Histogram: allows to use bars with different widths representing frequency distribution.
    {{< expand "Four main aspects of histograms" "" >}}
    1. Shape: overall shape of a histogram:
            - symmetric
            - bell-shaped (unimodal: has one peak)
            - left-skewed
            -right-skewed
    2. Center: mean or median
    3. Spread: how far the data spread:
        - Range
        - Interquartile Range (IQR)
        - standarn deviation
        - variance
    4. Outliers: data points that fall far from the bulk of the data


### Box Plot 

Box plot - also called a box-and-whisker plot


Boxplot represents a five-number summary:
1. Min: the smallest data point
2. Q1: the First Quartile, or the 25th percentile of the data
3. Centre: the **median**, so the distance between Q1 and Q3 gives us that middle 50 percent.
4. Q3: the Third Quartile, or the 75th percentile of the data
5. Max: largest data point

Min and max gives us a range.
Interquartile range: between Q1 and Q3.

### Histograms



## Standard deviation 

<!-- {{< katex >}}{SD=frac (o - m)/}{{< /katex >}} -->




## Assessment

1. Using the NHANES data and the previous notebook, the following questions will be about the variable BPXSY2 (with missing values remove). Round your answer to the nearest tenth. (ex: 2.33 should be 2.3, 2.15 should be 2.2)

What is the median?

2. What is the mean?

Round your answer to the nearest tenth. (ex: 2.33 should be 2.3, 2.15 should be 2.2)

3. What is the standard deviation?

Round your answer to the nearest tenth. (ex: 2.33 should be 2.3, 2.15 should be 2.2)

4. What is the standard deviation?

Round your answer to the nearest tenth. (ex: 2.33 should be 2.3, 2.15 should be 2.2)

5. What is the Interquartile Range (IQR)?

Round your answer to the nearest tenth. (ex: 2.33 should be 2.3, 2.15 should be 2.2)

6. Which of these will return descriptive statistics for a numeric Series ‘s’?

```python
s.describe()
Series.describe()
s.descriptive_stats()
describe(s)
```
7. Select all that apply: Which will produce a histogram of the numeric Series ‘s’
8. How many rows of the DataFrame 'df' are shown with the following code: 
`df.head()`

9. What data is shown when the following code is run?