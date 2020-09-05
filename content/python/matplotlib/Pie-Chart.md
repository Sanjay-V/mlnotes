---
title: "Pie Chart"
author: "Sanjay"
date: 2020-09-05
description: "-"
type: technical_note
draft: false
---

```python
# Importing Matplotlib library
from matplotlib import pyplot as plt 
```


```python
# Defining labels 
activities = ['eat', 'sleep', 'work', 'play']
```


```python
# Portion covered by each label 
slices = [4, 8, 7, 5] 
```


```python
# Color for each label 
colors = ['r', 'y', 'g', 'b'] 
```


```python
# Plotting the Pie chart 
plt.pie(slices, labels = activities, colors=colors, startangle=90, shadow = True, explode = (0, 0, 0.1, 0), 
        radius = 1.2, autopct = '%1.1f%%') 

# Plotting legend 
plt.legend() 

# Function to show the plot 
plt.show() 
```


![png](Pie-Chart_5_0.png)

