---
title: "Creating a Pandas Dataframe using string data"
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
# Importing StringIO function from io module 
from io import StringIO 
```


```python
# Wrap the string data in StringIO function and store it in a variable
data = StringIO("""Date;Exam;Marks 
10/2/2020;Maths;100 
11/2/2020;Physics;95
12/2/2020;Chemistry;80 
13/2/2020;ComputerScience;85 """) 
```


```python
# Read the data using Pandas read_csv() function 
data = pd.read_csv(data, sep =";") 
```


```python
# Print dataframe  
print(data) 
```

            Date             Exam  Marks 
    0  10/2/2020            Maths     100
    1  11/2/2020          Physics      95
    2  12/2/2020        Chemistry      80
    3  13/2/2020  ComputerScience      85

