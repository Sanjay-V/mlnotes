---
title: "Label Encoding"
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
# Importing Label Encoder from Sklearn
from sklearn.preprocessing import LabelEncoder 
le = LabelEncoder() 
```


```python
# Applying Label encoding for item column and printing it out
data['Item']= le.fit_transform(data['Item']) 
print(data['Item'])
```

    0    3
    1    4
    2    2
    3    1
    4    0
    Name: Item, dtype: int64



```python
# Printing label encoded dataframe
print(data)
```

       Item  Price
    0     3     85
    1     4     80
    2     2      5
    3     1     35
    4     0     30



```python
# Decoding the label encoded values
data['Item'] = le.inverse_transform(data['Item'])
print(data['Item'])
```

    0      Onion
    1     Tomato
    2        Egg
    3     Carrot
    4    Cabbage
    Name: Item, dtype: object

