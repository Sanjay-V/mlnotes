---
title: "Create a Pandas Series from scalar value"
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
# Initialize scalar value with indices
a = pd.Series(5, index=[0, 1, 2, 3])
```


```python
# Print Series values
print(a)
```

    0    5
    1    5
    2    5
    3    5
    dtype: int64

