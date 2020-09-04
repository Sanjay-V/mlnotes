---
title: "Conditional operation on Pandas Dataframe columns"
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
# Create pandas dataframe 
data = pd.DataFrame({'Date':['10/2/2020', '11/2/2020', '12/2/2020', '13/2/2020'], 
                   'Product':['Umbrella', 'Matress', 'Badminton', 'Shuttle'], 
                   'Last Price':[1200, 1500, 1600, 352], 
                   'Updated Price':[1300, 1400, 1550, 600], 
                   'Discount':[10, 10, 10, 10]}) 
```


```python
# Print the dataframe 
print(data) 
```

            Date    Product  Last Price  Updated Price  Discount
    0  10/2/2020   Umbrella        1200           1300        10
    1  11/2/2020    Matress        1500           1400        10
    2  12/2/2020  Badminton        1600           1550        10
    3  13/2/2020    Shuttle         352            600        10



```python
# Condition - Check if the updated price is available or not 
if 'Updated Price' in data.columns: 
    data['Final cost'] = data['Updated Price'] - (data['Updated Price']*0.1) 
  
else : 
    data['Final cost'] = data['Last Price'] - (data['Last Price']*0.1) 
```


```python
# Print the Dataframe 
print(data) 
```

            Date    Product  Last Price  Updated Price  Discount  Final cost
    0  10/2/2020   Umbrella        1200           1300        10      1170.0
    1  11/2/2020    Matress        1500           1400        10      1260.0
    2  12/2/2020  Badminton        1600           1550        10      1395.0
    3  13/2/2020    Shuttle         352            600        10       540.0

