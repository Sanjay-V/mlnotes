---
title: "Unary Operations"
author: "Sanjay"
date: 2020-09-04
description: "-"
type: technical_note
draft: false
---

```python
# Importing numpy library
import numpy as np
```


```python
# Creating array object
arr = np.array( [[ 71, 82, 53],
                 [ 48, 23, 56]] )
```


```python
# Printing the maximum element in a array
print("Largest element is:", arr.max())
```

    Largest element is: 82



```python
# Printing row-wise maximum elements
print("Row-wise maximum elements:", arr.max(axis = 1))
```

    Row-wise maximum elements: [82 56]



```python
# Printing column-wise maximum elements
print("Column-wise maximum elements:", arr.max(axis = 0))
```

    Column-wise maximum elements: [71 82 56]



```python
# Sum of array elements
print("Sum of all array elements:", arr.sum())
```

    Sum of all array elements: 333



```python
# Cumulative sum along each row of an array
print("Cumulative sum along each row of an array:\n",arr.cumsum(axis = 1))
```

    Cumulative sum along each row of an array:
     [[ 71 153 206]
     [ 48  71 127]]



```python
# Cumulative sum along each column of an array
print("Cumulative sum along each column of an array:\n",arr.cumsum(axis = 0))
```

    Cumulative sum along each column of an array:
     [[ 71  82  53]
     [119 105 109]]

