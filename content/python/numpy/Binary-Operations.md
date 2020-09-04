---
title: "Binary Operations"
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
# Creating array A
A = np.array( [[ 71, 82],
                 [ 48, 23]] )
```


```python
# Creating array B
B = np.array([[5, 2],
            [3, 7]])
```


```python
# Adding arrays and printing it out
print("Array sum:\n", A + B)
```

    Array sum:
     [[76 84]
     [51 30]]



```python
# Multiply arrays A and B (elementwise multiplication)
print("Array multiplication:\n", A*B)
```

    Array multiplication:
     [[355 164]
     [144 161]]



```python
# Multiply arrays A and B (matrix multiplication)
print("Matrix multiplication:\n", A.dot(B))
```

    Matrix multiplication:
     [[601 716]
     [309 257]]

