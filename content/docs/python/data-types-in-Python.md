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


{{< hint info >}} Markdown content
Dict in Python ordered since version 3.X {{< /hint >}}

# Methods

## Tuple methods

## Lists methods

| method | Example |
| ---------| ---------- |
| slice | `L[3:5]` 5 not included |
| append | add ONE element to the list. If a list is appended, it is added as one item - a nested list |
| extend | add many elements to the list |
| split | splits a string into a list. Add delimiter as a parameter to split on a specific character, e.g. by comma: `split(,)` |
| get items at an index range | Get the items stores at indexes 1 to 3 `my_list[1:4]` |



Clone list by value 

```python
list_B = list_A[:] 
list_B
``` 

Variable B references a new copy or clone of the original list.
Now if you change A, B will not change.



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
