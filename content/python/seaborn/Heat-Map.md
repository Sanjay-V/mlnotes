---
title: "Heat Map"
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
df = sns.load_dataset('tips') 
print(df)
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
# Correlation between the different parameters and printing it out
tc = df.corr() 
print(tc)
```

                total_bill       tip      size
    total_bill    1.000000  0.675734  0.598315
    tip           0.675734  1.000000  0.489299
    size          0.598315  0.489299  1.000000



```python
# Plot a heatmap for the correlated data 
sns.heatmap(tc) 

# Function to show the plot 
plt.show() 
```


![png](Heat-Map_4_0.png)
