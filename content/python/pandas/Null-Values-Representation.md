---
title: "Null Values Representation"
author: "Sanjay"
date: 2020-09-05
description: "-"
type: technical_note
draft: false
---

```python
# Import pandas library  
import pandas as pd
```


```python
# Initialize values with indices
a = pd.Series([1,2,3,4,5],index = ['a','c','e','f','i'])
```


```python
# Print the Pandas Series values
print(a)
```

    a    1
    c    2
    e    3
    f    4
    i    5
    dtype: int64



```python
# Reindexing the index
a = a.reindex(['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h'])
```


```python
# Print the Reindexed indices with values
print(a)
```

    a    1.0
    b    NaN
    c    2.0
    d    NaN
    e    3.0
    f    4.0
    g    NaN
    h    NaN
    dtype: float64



```python
# Print True for Null values to represent it
print(a.isnull())
```

    a    False
    b     True
    c    False
    d     True
    e    False
    f    False
    g     True
    h     True
    dtype: bool

