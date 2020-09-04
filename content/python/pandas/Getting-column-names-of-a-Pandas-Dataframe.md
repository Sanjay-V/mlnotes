---
title: "Getting column names of a Pandas Dataframe"
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
data = [{'Mark': 90, 'Grade': "O", 'Comments': "Best"}, 
        {'Mark': 75, 'Grade': "A", 'Comments': "Needs to be immproved"}]  
```


```python
# Print list of dicts 
print(data)
```

    [{'Mark': 90, 'Grade': 'O', 'Comments': 'Best'}, {'Mark': 75, 'Grade': 'A', 'Comments': 'Needs to be immproved'}]



```python
# Create the pandas DataFrame 
data = pd.DataFrame(data, index =['Stephen', 'Jerry']) 
```


```python
# Print dataframe  
print(data) 
```

             Mark Grade               Comments
    Stephen    90     O                   Best
    Jerry      75     A  Needs to be immproved



```python
# iterating the columns 
for col in data.columns: 
    print(col) 
```

    Mark
    Grade
    Comments

