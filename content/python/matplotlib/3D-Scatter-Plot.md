---
title: "3D Scatter Plot"
author: "Sanjay"
date: 2020-09-05
description: "-"
type: technical_note
draft: false
---

```python
# Import libraries 
from mpl_toolkits import mplot3d 
import numpy as np 
import matplotlib.pyplot as plt 
```


```python
# Creating dataset 
z = np.random.randint(100, size =(50)) 
x = np.random.randint(80, size =(50)) 
y = np.random.randint(60, size =(50)) 
```


```python
# Creating figure 
fig = plt.figure(figsize = (10, 7)) 
ax = plt.axes(projection ="3d") 
# Creating plot 
ax.scatter3D(x, y, z, color = "green")
plt.title("simple 3D scatter plot") 
# Function to show the plot 
plt.show() 
```


![png](3D-Scatter-Plot_3_0.png)

