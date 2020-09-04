---
title: "One Hot Encoding"
author: "Sanjay"
date: 2020-09-04
description: "-"
type: technical_note
draft: false
---

```python
# Import pandas and numpy library  
import pandas as pd
import numpy as np
```


```python
# Initialize list of dicts 
data = [{'Item': "Onion", 'Price': 85}, 
        {'Item': "Tomato", 'Price': 80},
       {'Item': "Egg", 'Price': 5},
       {'Item': "Carrot", 'Price': 35},
       {'Item': "Cabbage", 'Price': 30},] 
```


```python
# Print list of dicts 
print(data)
```

    [{'Item': 'Onion', 'Price': 85}, {'Item': 'Tomato', 'Price': 80}, {'Item': 'Egg', 'Price': 5}, {'Item': 'Carrot', 'Price': 35}, {'Item': 'Cabbage', 'Price': 30}]



```python
# Create the pandas DataFrame 
data = pd.DataFrame(data) 
```


```python
# Print dataframe  
print(data) 
```

          Item  Price
    0    Onion     85
    1   Tomato     80
    2      Egg      5
    3   Carrot     35
    4  Cabbage     30



```python
# Importing one hot encoder from sklearn 
from sklearn.preprocessing import OneHotEncoder 
ohe = OneHotEncoder() 
```


```python
# One hot encoding the Item column and printing it out
from sklearn.compose import ColumnTransformer 
columnTransformer = ColumnTransformer([('encoder', OneHotEncoder(), [0])], remainder='passthrough') 
datum = np.array(columnTransformer.fit_transform(data)) 
datum = pd.DataFrame(datum)
print(datum)
```

         0    1    2    3    4     5
    0  0.0  0.0  0.0  1.0  0.0  85.0
    1  0.0  0.0  0.0  0.0  1.0  80.0
    2  0.0  0.0  1.0  0.0  0.0   5.0
    3  0.0  1.0  0.0  0.0  0.0  35.0
    4  1.0  0.0  0.0  0.0  0.0  30.0



```python
# One hot encoding the dataset and printing it out
data = ohe.fit_transform(data).toarray()
data = pd.DataFrame(data)
print(data)
```

         0    1    2    3    4    5    6    7    8    9
    0  0.0  0.0  0.0  1.0  0.0  0.0  0.0  0.0  0.0  1.0
    1  0.0  0.0  0.0  0.0  1.0  0.0  0.0  0.0  1.0  0.0
    2  0.0  0.0  1.0  0.0  0.0  1.0  0.0  0.0  0.0  0.0
    3  0.0  1.0  0.0  0.0  0.0  0.0  0.0  1.0  0.0  0.0
    4  1.0  0.0  0.0  0.0  0.0  0.0  1.0  0.0  0.0  0.0

