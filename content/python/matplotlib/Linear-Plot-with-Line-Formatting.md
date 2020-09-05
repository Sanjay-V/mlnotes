---
title: "Linear Plot with Line Formatting"
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
# Assigning values 
Year = [1975, 1983, 1999, 2006, 2017] 
TamilNadu = [130.6, 158.61, 355.54, 384.76, 754.60] 
Assam = [10.4, 25.56, 58.75, 178.27, 254.87]
```


```python
# Formatting of line style and Plotting of co-ordinates 
plt.plot(Year, TamilNadu, color ='orange', marker ='o', markersize = 10, label ='Tamil Nadu') 
plt.plot(Year, Assam, color ='g', linestyle ='dashed', linewidth = 3, label ='Assam') 
# Labelling the plot
plt.xlabel('Years') 
plt.ylabel('Income in crores') 
plt.title('Income of Tamil Nadu and Assam') 
plt.legend() 
# Function to show the plot 
plt.show() 
```


![png](Linear-Plot-with-Line-Formatting_3_0.png)

