---
title: "Working with Text Data"
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
# Initialize values with Pandas Series
a = pd.Series(['Tom', 'William Rick', 'John', 'Albert', '1234', 'SteveSmith'])
```


```python
# Print Pandas Series values
print(a)
```

    0             Tom
    1    William Rick
    2            John
    3          Albert
    4            1234
    5      SteveSmith
    dtype: object



```python
# Calling lower() built-in function and printing the values
print(a.str.lower())
```

    0             tom
    1    william rick
    2            john
    3          albert
    4            1234
    5      stevesmith
    dtype: object



```python
# Calling upper() built-in function and printing the values
print(a.str.upper())
```

    0             TOM
    1    WILLIAM RICK
    2            JOHN
    3          ALBERT
    4            1234
    5      STEVESMITH
    dtype: object



```python
# Calling len() built-in function and printing the values
print(a.str.len())
```

    0     3
    1    12
    2     4
    3     6
    4     4
    5    10
    dtype: int64

