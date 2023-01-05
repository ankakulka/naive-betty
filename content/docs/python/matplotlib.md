---
title: "Matplotlib"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---



Matplotlib is a plotting library. In this section give a brief introduction to the matplotlib.pyplot module.

## Installation 

Install via pip: 

```
pip install matplotlib
```


## Import

As Matplotlib builds on the NumPy library, you have to import both.
<!-- Check if this is def the case -->

```python
import numpy as np
import matplotlib.pyplot as plt
```

### Create a basic plot

```python
# Compute the x and y coordinates for points on a sine curve
x = np.arange(0, 3 * np.pi, 0.1)
y = np.sin(x)

# Plot the points using matplotlib
plt.plot(x, y)
plt.show()  # You must call plt.show() to make graphics appear.

```