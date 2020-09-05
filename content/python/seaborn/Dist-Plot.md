---
title: "Dist Plot"
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
# Load the in-built dataset and printing it out
data = sns.load_dataset('tips') 
print(data)
```

         total_bill   tip     sex smoker   day    time  size
    0         16.99  1.01  Female     No   Sun  Dinner     2
    1         10.34  1.66    Male     No   Sun  Dinner     3
    2         21.01  3.50    Male     No   Sun  Dinner     3
    3         23.68  3.31    Male     No   Sun  Dinner     2
    4         24.59  3.61  Female     No   Sun  Dinner     4
    ..          ...   ...     ...    ...   ...     ...   ...
    239       29.03  5.92    Male     No   Sat  Dinner     3
    240       27.18  2.00  Female    Yes   Sat  Dinner     2
    241       22.67  2.00    Male    Yes   Sat  Dinner     2
    242       17.82  1.75    Male     No   Sat  Dinner     2
    243       18.78  3.00  Female     No  Thur  Dinner     2
    
    [244 rows x 7 columns]



```python
# Set the background style of the plot 
sns.set_style('whitegrid') 
```


```python
# Plotting Dist plot with Seaborn 
sns.distplot(data['total_bill'], kde = False, color ='red', bins = 30) 
  
# Giving title to the plot 
plt.title('Tips per week') 
  
# Function to show the plot 
plt.show() 
```


![png](Dist-Plot_4_0.png)

