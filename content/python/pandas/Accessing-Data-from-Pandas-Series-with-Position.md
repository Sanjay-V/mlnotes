---
title: "Accessing Data from Pandas Series with Position"
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
# Print Series first element value
print(a[0])
```

    1



```python
# Print Series third element value
print(a[2])
```

    3

