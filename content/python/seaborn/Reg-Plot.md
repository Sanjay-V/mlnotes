---
title: "Reg Plot"
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
df = sns.load_dataset('mpg') 
print(df)
```

          mpg  cylinders  displacement  horsepower  weight  acceleration  \
    0    18.0          8         307.0       130.0    3504          12.0   
    1    15.0          8         350.0       165.0    3693          11.5   
    2    18.0          8         318.0       150.0    3436          11.0   
    3    16.0          8         304.0       150.0    3433          12.0   
    4    17.0          8         302.0       140.0    3449          10.5   
    ..    ...        ...           ...         ...     ...           ...   
    393  27.0          4         140.0        86.0    2790          15.6   
    394  44.0          4          97.0        52.0    2130          24.6   
    395  32.0          4         135.0        84.0    2295          11.6   
    396  28.0          4         120.0        79.0    2625          18.6   
    397  31.0          4         119.0        82.0    2720          19.4   
    
         model_year  origin                       name  
    0            70     usa  chevrolet chevelle malibu  
    1            70     usa          buick skylark 320  
    2            70     usa         plymouth satellite  
    3            70     usa              amc rebel sst  
    4            70     usa                ford torino  
    ..          ...     ...                        ...  
    393          82     usa            ford mustang gl  
    394          82  europe                  vw pickup  
    395          82     usa              dodge rampage  
    396          82     usa                ford ranger  
    397          82     usa                 chevy s-10  
    
    [398 rows x 9 columns]



```python
# Plot Reg Plot for the data 
sns.regplot(x = "mpg", y = "acceleration", data = df) 

# Function to show the plot 
plt.show() 
```


![png](Reg-Plot_3_0.png)

