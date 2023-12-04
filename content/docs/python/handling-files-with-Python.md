---
title: "Handling Files With Python"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

## Opening Files

Use `with open() as` method:

```python
with open('example.txt','r') as testfile:
    print(testfile.read())
```

Thanks to this method you don't have to close the file, as required when using just `open`.

## Read Files


### Read line

`.readline()`


## Writing Files

Write file

```python
exmp2 = '/Example2.txt'
with open(exmp2, 'w') as writefile:
    writefile.write("This is line A")
```

Write line to a file

```python

```

## Append Files

We can write to files without losing any of the existing data as follows by setting the mode argument to append: a. you can append a new line as follows

```python
with open('/Example2.txt', 'a') as testwritefile:
    testwritefile.write("This is line C\n")
    testwritefile.write("This is line D\n")
    testwritefile.write("This is line E\n")

```


## Combined methods

Most of the file methods we've looked at work in a certain location in the file. .write() writes at a certain location in the file. .read() reads at a certain location in the file and so on. You can think of this as moving your pointer around in the notepad to make changes at specific location.

Opening the file in w is akin to opening the .txt file, moving your cursor to the beginning of the text file, writing new text and deleting everything that follows. Whereas opening the file in a is similiar to opening the .txt file, moving your cursor to the very end and then adding the new pieces of text.
It is often very useful to know where the 'cursor' is in a file and be able to control it. The following methods allow us to do precisely this -

`.tell()` - returns the current position in bytes
`.seek(offset,from)` - changes the position by 'offset' bytes with respect to 'from'. From can take the value of 0,1,2 corresponding to beginning, relative to current position and end




## File modes table




| Syntax      | Mode |
| ----------- | ----------- |
| `r`   | read      |
| `w`  | write        | 
| `a`  | append       | 
| `x` | exclusive creation |
| `wb` | write binary |
| `ab` | append bnary |
| `xb` | exclusive binary creation |
| `rt` | read text | 
| `wt` | write text |
| `xt` | exclusive text creation |
| `r+` | Reading and writing: Cannot truncate the file. |
|  `w+`  | Writing and reading: Truncates the file |
|  `a+`   | Appending and Reading: Creates a new file, if none exists |

