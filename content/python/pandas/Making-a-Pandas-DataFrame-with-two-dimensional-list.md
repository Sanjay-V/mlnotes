---
title: "Making a Pandas DataFrame with two-dimensional list"
author: "Sanjay"
date: 2020-08-11
description: "-"
type: technical_note
draft: false
---

```python
import pandas as pd
```


```python
lst = [['Nicole', 'Williamson', 23], ['William', 'Smith', 29],  
       ['Nick', 'Fury', 30], ['Vin', 'williams', 22]] 
```


```python
print(lst)
```

    [['Nicole', 'Williamson', 23], ['William', 'Smith', 29], ['Nick', 'Fury', 30], ['Vin', 'williams', 22]]



```python
df = pd.DataFrame(lst, columns =['FirstName', 'LastName', 'Age'])  
```


```python
print(df)
```

      FirstName    LastName  Age
    0    Nicole  Williamson   23
    1   William       Smith   29
    2      Nick        Fury   30
    3       Vin    williams   22

