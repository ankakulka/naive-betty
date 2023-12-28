---
title: "Matplotlib"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
type: "page"
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

### Create a basic line plot

The simplest and most fundamental plot is a standard line plot. The function expects two arrays as input, x and y, both of the same size. x is treated as an independent variable and y as the dependent one. The graph is plotted as shortest line segments joining the x,y point pairs ordered in terms of the variable x.

```python
# Compute the x and y coordinates for points on a sine curve
x = np.arange(0, 3 * np.pi, 0.1)
y = np.sin(x)

# Plot the points using matplotlib
plt.plot(x, y)
plt.show()  # You must call plt.show() to make graphics appear.

```

### Scatter plot

Scatter plots are graphs that present the relationship between two variables in a data set. It represents data points on a two-dimensional plane. The independent variable or attribute is plotted on the X-axis, while the dependent variable is plotted on the Y-axis.

Use scatter plots when:
- you have paired numerical data
- unique value of an independent variable corresponds to multiple values of the dependent variable
- to determine relationship between variables

```python

plt.scatter(x,y)

```


### Histogram

A histogram is an important visual representation of data in categorical form. To view the data in a "Binned" form, we may use the histogram plot with a number of bins required or even with the data points that mark the bin edges. The x-axis represents the data bins, and the y-axis represents the number of elements in each of the bins.

```python

plt.hist(x, bins)

```

Use an additional argument, edgecolor, for better clarity of plot.
Consider the graph shown below. The left graph is the histogram plot for a data set, plotted without setting the edgecolor. The right one is the same graph but has the edgecolor argument set as the color black.


### Bar plot

A bar plot is used for visualizing catogorical data. The y-axis represents the average value of data points belonging to a particular category, while the x-axis represents the number of elements in the different categories. 

```python

plt.bar(x, height)

```

x is the categorical variable, and height is the number of values belonging to the category. You can adjust the width of each bin using an additional width argument in the function.

### Pseudocolor plot

A pseudocolor plot displays matrix data as an array of colored cells (known as faces). This plot is created as a flat surface in the x-y plane. The surface is defined by a grid of x and y coordinates that correspond to the corners (or vertices) of the faces. Matrix C specifies the colors at the vertices. The color of each face depends on the color of one of its four surrounding vertices. Of the four vertices, the one that comes first in the x-y grid determines the color of the face.

```python

plt.pcolor(c)

```

Add `cmap` argument to specify the color scheme of the plot. 