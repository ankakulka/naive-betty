---
title: "Errors and Exceptions in Python"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Handling Error and Exceptions in Python

Errors are usually problems that come from the computer or the system. Exceptions are more like issues we can control. Usually they can be fixed, so the program keeps going.

## Generic exceptions:

```python
try:
    # code to try to execute
except:
    # code to execute if there is an exception


```

## Specific exceptions

Common Built-in Python exceptions

| Exception | Occurs...|
|-----------|-------------|
| `ZeroDivisionError` |  if division by zero is attempted |
| `ValueError` | when inappropriate value is used. For example, converting non-numeric string to integer |
| `FileNotFoundError ` | if file does not exist  |
| `IndexError` | when accesing element in a list that is outside of a valid index range |
| `KeyError` | whenaccessing non-existent key in a dictionary |
| `TypeError` |  when object is used in an incompatible manner. An example includes trying to concatenate a string and an integer |
| `AttributeError` | when accessing attribute or method non-existing on that object |
| `ImportError` | when importing a module that is unavailable |


<!-- [Python Documentation](https://docs.python.org/3/library/exceptions.html#) lists all exceptions.  -->

### Specific exception example code

```python
# using Try- except 
try:
    # Attempting to divide 10 by 0
    result = 10 / 0
except ZeroDivisionError:
    # Handling the ZeroDivisionError and printing an error message
    print("Error: Cannot divide by zero")
# This line will be executed regardless of whether an exception occurred
print("outside of try and except block")

```

Try except **else**  allows one to check if there was no exception when executing the try block. This is useful when we want to execute something only if there were no errors.

```python
# potential code before try catch

try:
    # code to try to execute
except ZeroDivisionError:
    # code to execute if there is a ZeroDivisionError
except NameError:
    # code to execute if there is a NameError
except:
    # code to execute if ther is any exception
else:
    # code to execute if there is no exception
    
# code that will execute if there is no exception or a one that we are handling

```

`finally` allows us to always execute something even if there is an exception or not. This is usually used to signify the end of the try except.

```python
# potential code before try catch

try:
    # code to try to execute
except ZeroDivisionError:
    # code to execute if there is a ZeroDivisionError
except NameError:
    # code to execute if there is a NameError
except:
    # code to execute if ther is any exception
else:
    # code to execute if there is no exception
finally:
    # code to execute at the end of the try except no matter what
    
# code that will execute if there is no exception or a one that we are handling

```

