---
title: "Array Operations"
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
# Defining Array A
A = np.array([[17, 23],
              [34, 46]])
```


```python
# Defining Array B
B = np.array([[48, 39],
              [25, 14]])
```


```python
# Adding 5 to every element in Array A
print("Adding 5 to every element in Array A:", A + 5)
```

    Adding 5 to every element in Array A: [[22 28]
     [39 51]]



```python
# Subtracting 2 from each element
print("\nSubtracting 2 from each element of Array B:", B - 2)
```

    
    Subtracting 2 from each element of Array B: [[46 37]
     [23 12]]



```python
# Sum of Array A elements performing Unary operations
print ("\nSum of all array A elements: ", A.sum())
```

    
    Sum of all array A elements:  120



```python
# Adding two arrays A and B performing Binary operations
print ("\nArray sum:\n", A + B)
```

    
    Array sum:
     [[65 62]
     [59 60]]

