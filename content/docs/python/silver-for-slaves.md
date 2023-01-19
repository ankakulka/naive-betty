---
title: "Silver for Slaves"
weight: 1
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# Visit to the silver for slaves exhibition

A visit to the Silver for Slaves exhibition at the Silesian Museum in Gorlitz has impressed me and inspired to look further into the data I found overthere. 
The price that would be paid for certain items such as live stock, artefacts or slaves is something th

To see a price of foodstuffs, livestock and artefacts alongside prices for a slave is shocking. It is even more shocking to see how the price of a slave compares to other prices. This sort of information is something that is best presented visually, so 
I wanted to create a simple chart using `matplotlib` package. 



```python
import numpy as np
import matplotlib.pyplot as plt
```


I created a dictionary containing the data I collected at the exhibition:

```python
silver = {"knife":1,"sheep":15,"lance":51,"pig":30,"man slave":306,"chain male":804}
```

To create a basic bar chart in Python: 

```python
keys = silver.keys()
values = silver.values()

plt.bar(keys, values)
```

```python
x = silver.keys()
y = silver.values()

plt.xlabel('Items')
plt.ylabel('Grams of Silver')
plt.title('Amount of Silver in Gram paid in the Middle Ages')

plt.bar(x, y)
```