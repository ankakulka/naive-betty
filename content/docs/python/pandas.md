---
title: "Pandas"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Pandas

Pandas is a popular Python library used to handle data, statistical functions and ...
Pandas offers two primary data structures - DataFrame and Series.

## Data Import and Export: 


Pandas makes it easy to read data from various sources, including CSV files, Excel spreadsheets, SQL databases, and more. It can also export data to these formats, enabling seamless data exchange.

### Read a CSV file

```python

df = pd.read_csv('your_file.csv')

```


## Data Merging and Joining

You can combine multiple DataFrames using methods like merge and join, similar to SQL operations, to create more complex datasets from different sources.


## Efficient Indexing

Pandas provides efficient indexing and selection methods, allowing you to access specific rows and columns of data quickly.

# Custom Data Structures

You can create custom data structures and manipulate data in ways that suit your specific needs, extending Pandas' capabilities.

## Data Frame

A DataFrame is a two-dimensional, size-mutable, and potentially heterogeneous tabular data structure with labeled axes (rows and columns).


### Creating a DataFrame from a dictionary

DataFrames can be created from dictionaries, with keys as column labels and values as lists representing rows.


```python

data = {'Name': ['Alice', 'Bob', 'Charlie', 'David'],
        'Age': [25, 30, 35, 28],
        'City': ['New York', 'San Francisco', 'Los Angeles', 'Chicago']}
df = pd.DataFrame(data)

```


You can select a single column from a DataFrame by specifying the column name within double brackets.
Multiple columns can be selected in a similar manner, creating a new DataFrame.

You can access rows by their index using .iloc[] or by label using .loc[].

### Find unique item in A Data Frame

`unique_dates = df['Age'].unique()`

### Filtering Data Frames

You can filter data in a DataFrame based on conditions using inequality operators.
For instance, you can filter albums released after a certain year.

`high_above_102 = df[df['Age'] > 25]`

### Saving Data Frame

`df.to_csv('trading_data.csv', index=False)`

## Series

A Series is a one-dimensional labeled array, essentially a single column or row of data.
A Series is a one-dimensional labeled array in Pandas. It can be thought of as a single column of data with labels or indices for each element. You can create a Series from various data sources, such as lists, NumPy arrays, or dictionaries



## Attributes and Methods: Extract

### General methods

| method | Displays |
| -------- | ------------ |
| shape | dimensions (number of rows and columns) of the DataFrame |
| info() |  summary of the DataFrame, including data types and non-null counts |
| describe() | summary statistics for numerical columns |
| head() | first row |
| tail() | last row |

### Calculation methods

| method | Calculates |
| -------- | -------- |
| mean() | mean  |
| sum() |  sum | 
|  min() |    |
| max() |    |

### Other methods

- sort_values(): Sort the DataFrame by one or more columns.
- groupby(): Group data based on specific columns for aggregation.
- fillna(), drop(), rename(): Handle missing values, drop columns, or rename columns.
- apply(): Apply a function to each element, row, or column of the DataFrame.