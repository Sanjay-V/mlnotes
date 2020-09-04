---
title: "Creating a Pandas Dataframe using list of tuples"
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
# Initialize list of tuples
lst = [('Numpy', 10), ('Pandas', 15), ('Matplotlib', 20), ('Scikit-Learn', 25)]  
```


```python
# Print list of tuples 
print(lst)
```

    [('Numpy', 10), ('Pandas', 15), ('Matplotlib', 20), ('Scikit-Learn', 25)]



```python
# Create the pandas DataFrame 
data = pd.DataFrame(lst, columns = ['Tech', 'Points']) 
```


```python
# Print dataframe  
print(data) 
```

               Tech  Points
    0         Numpy      10
    1        Pandas      15
    2    Matplotlib      20
    3  Scikit-Learn      25

