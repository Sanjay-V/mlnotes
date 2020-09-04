---
title: "Dropping columns of a Pandas Dataframe"
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
# Dropping column of dataframe
data = data.drop(['Last Price'], axis = 1) 
```


```python
# Print the Dataframe 
print(data) 
```

            Date    Product  Updated Price  Discount
    0  10/2/2020   Umbrella           1300        10
    1  11/2/2020    Matress           1400        10
    2  12/2/2020  Badminton           1550        10
    3  13/2/2020    Shuttle            600        10

