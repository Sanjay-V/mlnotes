---
title: "Getting unique values from a column in Pandas Dataframe"
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
        {'Mark': 75, 'Grade': "A", 'Comments': "Needs to be immproved"},
       {'Mark': 40, 'Grade': "F", 'Comments': "Hard work is essential"}]  
```


```python
# Print list of dicts 
print(data)
```

    [{'Mark': 90, 'Grade': 'O', 'Comments': 'Best'}, {'Mark': 75, 'Grade': 'A', 'Comments': 'Needs to be immproved'}, {'Mark': 40, 'Grade': 'F', 'Comments': 'Hard work is essential'}]



```python
# Create the pandas DataFrame 
data = pd.DataFrame(data, index =['Stephen', 'Jerry', 'Robert']) 
```


```python
# Print dataframe  
print(data) 
```

             Mark Grade                Comments
    Stephen    90     O                    Best
    Jerry      75     A   Needs to be immproved
    Robert     40     F  Hard work is essential



```python
# Getting unique values of a column in a dataframe
mark = data.Mark.unique()
print(list(mark))
```

    [90, 75, 40]



```python
# Getting number of unique values of a column in a dataframe
a = data.Mark.nunique()
print(a)
```

    3

