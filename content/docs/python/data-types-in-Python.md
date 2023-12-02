---
title: "Data Types in Python"
weight: 1
draft: flase
bookToc: true
# bookFlatSection: false
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Comparison table of data structures in Python

| Data Type   | Syntax |  Index       | Mutable    | Duplicates |
| ----------- | ----------- | ----------- | ----------- |----------- | 
| Tuple       | ```python tup = (val1, val2, val3)``` | ?           | NO | ? |
| List        | ```python my_list = [val1, val2, val3]```   | YES     | YES | YES |
| Set         | ```python my_set = {some_val, another_val}```  | NO       | NO | NO|
| Dictionary  | ```python dict = {key: value}```        | YES\*        | YES | NO |

# Methods

## Tuple methods

## Lists methods



## Dictionary and sets methods

| Method | Example |
|--------|--------- |
| add     | `fruits.add("mango")` |
| clear |  `fruits.clear()</td>` |
| copy   | `new_fruits = fruits.copy()` |
| discard | ` ` |
| issubset | ` ` |
| issuperset | `` |
| pop | The `pop()` method removes and returns an arbitrary element from the set. It raises a `KeyError` if the set is empty. Use this method to remove elements when the order doesn't matter.`` |
| remove | Use the `remove()` method to remove a specific element from the set. Raises a `KeyError` if the element is not found `` |
| update | adds elements from another iterable into the set. It maintains the uniqueness of elements. `set_name.update(iterable) ` `fruits.update(["kiwi", "grape"])` |


### Set Operations

Perform various operations on sets: `union`, `intersection`, `difference`, `symmetric difference`

```python
union_set = set1.union(set2) 
intersection_set = set1.intersection(set2) 
difference_set = set1.difference(set2) 
sym_diff_set = set1.symmetric_difference(set2) 

```
