---
title: "Retrieve the first three elements in Pandas Series"
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
# Print the retrieved first three elements in Pandas Series
print(a[:3])
```

    a    1
    b    2
    c    3
    dtype: int64

