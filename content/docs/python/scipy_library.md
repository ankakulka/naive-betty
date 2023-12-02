---
title: "Scipy Library"
weight: 1
# bookFlatSection: false
bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
type: "page"
---

# Intro to SciPy Library

https://scipy.org/

>is an open-source software for mathematics, science, and engineering.

[SciPy docs](https://docs.scipy.org/doc/scipy/)

The SciPy library builds on the NymPy's library multidimentional arrays and offers a large number of functions that operate on them. 

It is useful for different types of scientific and engineering applications. 
 
The SciPy.stats sub-library. Within the .stats sub-library, we see functions for continuous and discreet distributions, descriptive statistics, and also statistical test such as T-test. Now let's get into some of these uses.

## Installation 

Install via pip: 

```
pip install scipy
```

## Import

As SciPy builds on the NumPy library, you have to import both.
We're importing the `stats` module only which contains statistical functions.

```python
from scipy import stats
import numpy as np
```

## Working with Scipy 

The SciPy.Stats module contains a large number of probability distributions as well as a growing library of statistical functions such as:

- Continuous and Discrete Distributions (i.e Normal, Uniform, Binomial, etc.)
- Descriptive Statistcs
- Statistical Tests (i.e T-Test)

### Generating random variables

Use the dot operator and call normal rvs, which means we're going to create normal random variables and we'll specify a size, and what that does is it states we want ten normal random variables.

```python

print(stats.norm.rvs(size = 10))

```

Outputs an array of ten random floats: 

```python
[-1.87444477 -2.52986741  1.20213559  0.90137446  0.77705937 -0.4185372
  0.05714971  1.41299781 -0.5249351  -0.81897983]
```


### Descriptive statistics

```python

np.random.seed(282629734)
x = stats.t.rvs(10, size=1000)

```
Do some descriptive statistics:

```python

print(x.min())   # equivalent to np.min(x)

print(x.max())   # equivalent to np.max(x)

print(x.mean())  # equivalent to np.mean(x)

print(x.var())   # equivalent to np.var(x))

stats.describe(x)

```



### PDF: Probability density function 

Probability density functions are a statistical measure used to gauge the likely outcome of a discrete value. PDFs are plotted on a graph typically resembling a bell curve, with the probability of the outcomes lying below the curve.

The normal distribution is a common example of a PDF, forming the well-known bell curve shape.

### CDF:  Cumulative density function 

