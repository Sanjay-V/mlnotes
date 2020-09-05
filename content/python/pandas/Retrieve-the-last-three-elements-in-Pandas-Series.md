---
title: "Retrieve the last three elements in Pandas Series"
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
a = pd.Series([1,2,3,4,5],index = ['a','b','c','d','e'])
```


```python
# Print the retrieved last three elements in Pandas Series
print(a[-3:])
```

    c    3
    d    4
    e    5
    dtype: int64

