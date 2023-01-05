---
title: "NumPy Library Intro"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
toc: true
---



# Intro to  NumPy Python Library

Numpy official documentation: 

> The fundamental package for scientific computing with Python.

> NumPy doesn’t depend on any other Python packages, however, it does depend on an accelerated linear algebra library - typically Intel MKL or OpenBLAS. Users don’t have to worry  about installing those 

For the basics intro see: https://numpy.org/devdocs/user/quickstart.html

## Installation 

Via conda or pip: 

```
pip install numpy
```

## Import

Customary way to import: 

```python
import numpy as np
```

## Numpy Arrays


A NumPy array is a grid of values, all of the same type, and is indexed by a tuple of nonnegative integers.
The number of dimensions is the rank of the array.
The shape of the array is the tuple of integers giving the size of the array along each dimension.

```python
basic_array = np.array([1,2,3])
```

### Shape of the array

The shape of the array gives you the dimesions and the number of values. 
Use the dot function to acces the shape of the array:

```python
print(np.shape(test_array))

```

### Create an array with same values

NumPy gives a functionality of creating an array containint the same values.

1. An array containing zeros only. The input are the dimensions of the array: 

```python

zero_array = np.zeros((3, 2))
# (3,2) specifies the dimensions of the array

```

2. An array containing ones only: 

```python

ones_array = np.ones((3, 2))
# (3,2) specifies the dimensions of the array

```
Full constant array with specified value

```python
constant_values = np.full((3,3), 9)
# (3,3) specifies the dimensions of the array
# 9 specifies the constant value

```


### Random array 

Create a random array with dimensions 3x3: 

```python

random_array = np.random.random((3,3))
print(random_array)

```

Examle of a random array 

```python
[[0.78901706 0.24720225 0.27769623]
 [0.27916406 0.80738536 0.13918108]
 [0.15035761 0.02093592 0.93843837]]
```

### Accessing individual values in an array

```python
print(random_array[0,0])

# prints

0.7890170614173391

```


### Get the values of the NumPy array



### Slicing a NumPy array





