---
title: "Creating a Pandas Dataframe using list of dicts"
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
data = [{'Raghul': 90, 'Ramesh': 85, 'Steven': 70}, 
        {'Raghul': 'O', 'Ramesh': 'A+', 'Steven': 'A'}]  
```


```python
# Print list of dicts 
print(data)
```

    [{'Raghul': 90, 'Ramesh': 85, 'Steven': 70}, {'Raghul': 'O', 'Ramesh': 'A+', 'Steven': 'A'}]



```python
# Create the pandas DataFrame 
data = pd.DataFrame(data, index =['Marks', 'Grade']) 
```


```python
# Print dataframe  
print(data) 
```

          Raghul Ramesh Steven
    Marks     90     85     70
    Grade      O     A+      A

