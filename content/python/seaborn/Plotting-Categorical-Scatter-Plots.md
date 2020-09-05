---
title: "Plotting Categorical Scatter Plots"
author: "Sanjay"
date: 2020-09-05
description: "-"
type: technical_note
draft: false
---

```python
# Importing the Matplotlib and Seaborn library
import matplotlib.pyplot as plt 
import seaborn as sns 
```


```python
# Assigning x axis values 
x =['Sun', 'Mon', 'Tues', 'Wednes', 'Thurs', 'Fri', 'Satur'] 
```


```python
# Assigning y axis values 
y =[5, 6, 4, 6.5, 2.3, 4.9, 8.8] 
```


```python
# Plotting Strip plot with Seaborn 
a = sns.stripplot(x, y)

# Giving labels to x-axis and y-axis 
a.set(xlabel ='Days', ylabel ='Work-Load') 
  
# Giving title to the plot 
plt.title('Works per week')
  
# Function to show the plot 
plt.show() 
```


![png](Plotting-Categorical-Scatter-Plots_4_0.png)

