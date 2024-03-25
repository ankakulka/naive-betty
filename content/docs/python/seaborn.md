---
title: "Seaborn"
weight: 1
# bookFlatSection: false
bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
type: "page"
---

# Introduction to Seaborn Library


Seabord comes with in-built "Penguins" dataset.

## Install/Import libraries

```python
import seaborn as sn
import matplotlib.pyplot as plt
```

Access it by using `load_dataset` method:

```python
df = sn.load_dataset('penguins')
```

Using `describe()` method, familiarise yourself with the data:


To create a simplest scatter plot, add the x and y axis. 

```python

sn.relplot(data=df, x='body_mass_g', y='flipper_length_mm')

```


Final code

```python
sn.relplot(data=df, x='body_mass_g', y='flipper_length_mm', hue='sex', size="bill_length_mm", sizes=(10, 100), alpha=0.5)
sn.set_palette('Set2')
sn.set_style('darkgrid')
plt.xlabel("body mass")
plt.ylabel("flipper length")
plt.title("Penguins Body Mass vs Flipper Length")
# When working in IDE rather than in Jupyter notebook, add:
plt.show()
```


### Seaborn Color palettes

https://seaborn.pydata.org/tutorial/color_palettes.html

### Matplotlib Markers

Change the style of the marker from the default circle to:
-trinagle (up/down)
- square
- star
- hexagon

For the full list, go to: https://matplotlib.org/stable/api/markers_api.html