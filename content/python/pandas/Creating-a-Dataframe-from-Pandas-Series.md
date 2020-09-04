---
title: "Creating a Dataframe from Pandas Series"
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
# Initialize lists values
students = ['Steven', 'James', 'Ronald', 'Han'] 
marks = [90, 95, 65, 73] 
```


```python
# Print students list values
print(student)
```

    ['Steven', 'James', 'Ronald', 'Han']



```python
# Print marks list values
print(marks)
```

    [90, 95, 65, 73]



```python
# Importing Series from Pandas for students list and printing it out
students = pd.Series(students) 
marks = pd.Series(marks)
print(students)
```

    0    Steven
    1     James
    2    Ronald
    3       Han
    dtype: object



```python
# Importing Series from Pandas for marks list and printing it out
marks = pd.Series(marks) 
print(marks)
```

    0    90
    1    95
    2    65
    3    73
    dtype: int64



```python
# Converting list values into dictionary values
data = { 'Students': students, 'Marks': marks } 
print(data)
```

    {'Students': 0    Steven
    1     James
    2    Ronald
    3       Han
    dtype: object, 'Marks': 0    90
    1    95
    2    65
    3    73
    dtype: int64}



```python
# Creating Dataframe from dictionary values
data = pd.DataFrame(data) 
print(data)
```

      Students  Marks
    0   Steven     90
    1    James     95
    2   Ronald     65
    3      Han     73



```python
# Adding external grades list and printing it out
grades = ["A+", "O", "B+", "A"] 
print(grades)
```

    ['A+', 'O', 'B+', 'A']



```python
# Adding grades list to the created dataframe
data['Grades'] = pd.Series(grades)
```


```python
# Print the dataframe
print(data)
```

      Students  Marks Grades
    0   Steven     90     A+
    1    James     95      O
    2   Ronald     65     B+
    3      Han     73      A

