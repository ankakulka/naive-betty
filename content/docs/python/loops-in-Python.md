---
title: "Loops in Python"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# For loops

Use for loops when you know the number of iterations in advance and want to process each element in a sequence. They are best suited for iterating over collections and sequences where the length is known.

In Python, you can easily iterate over a data structure such as a list and print all of its items: 

```python
colors = ["red", "orange", "yellow", "green", "blue", "indigo", "violet"]

for color in colours:
    print(color)

```

Also works for a tuple/ set/ dictionary. 

Beware - this loops over the dictionary **keys** not values. 
```python
dict = {"hat": "red", "shirt":"orange"}
for color in dict:
    print(color)
```
prints: `hat shirt` 

<!-- To print the dictionary values: -->


## For range

Python offers a very convenient range function. By default it starts at 0, not including the given number. 

1. Print 0 to 10

    ```python
    for i in range(11):
        print(i)
    ```

2. Print 1 to 10
    ```python
    for i in range(1, 11):
        print(i)
    ```
3. Print 25 to 39
    ```python 
    for i in range(25, 39):
        print(i)
    
    ```

Only works for numbers. 

### Generate a list of the alphabet in Python with a for loop

```python
alphabet = []
for i in range(97, 123):
    alphabet.append(chr(i))

print(alphabet)
```


Print a list of all letters of the alphabet in uppercase; use string module and ascii method.

```python
alphabet = list(string.ascii_uppercase)
print(alphabet)
```

# While loop

Use while loops when you need to perform a task repeatedly as long as a certain condition holds true. While loops are particularly useful for situations where the number of iterations is uncertain or where you're waiting for a specific condition to be met. 

Print numbers from 0 to 11

```python
i = 0
while i < 11:
    print(i)
    i += 1
```

Print numbers from 1 to 10:
```python
i = 1
while i < 11:
    print(i)
    i += 1
```

Print numbers from 0 to -10

```python
i = 0
while i > -11:
    print(i)
    i -= 1
```

Print every second number from 2 to 10
```python
i = 2
while i < 11:
    print(i)
    i += 2
```

Print all the values from the list: 
```python


```



## Enumerate function

You can easily get the index and the item using the enumerate method.
Use it for tuples, list.

If used with a set duplicates are omitted. If used with a dictionary, loops over the keys, not values. 

```python
fruits = ("apple", "banana", "orange")

RGB = ("red", "green", "blue")
for index, color in enumerate(RGB):
    print(f"At position {index}, I found {color}")
```


