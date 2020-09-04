---
title: "Creating Pandas Dataframe using list of lists"
author: "Sanjay"
date: 2020-09-04
description: "-"
type: technical_note
draft: false
---

```python
# Import pandas library  
import pandas as pd
```


```python
# Initialize list of lists 
lst = [['Numpy', 10], ['Pandas', 15], ['Matplotlib', 20]]  
```


```python
# Print list of lists 
print(lst)
```

    [['Numpy', 10], ['Pandas', 15], ['Matplotlib', 20]]



```python
# Create the pandas DataFrame 
data = pd.DataFrame(lst, columns = ['Tech', 'Points']) 
```


```python
# Print dataframe  
print(data) 
```

             Tech  Points
    0       Numpy      10
    1      Pandas      15
    2  Matplotlib      20

