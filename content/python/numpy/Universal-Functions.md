---
title: "Universal Functions"
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
# Printing an array of sine values
print("Sine values of array elements:", np.sin(A))
```

    Sine values of array elements: [[ 0.95105465  0.31322878]
     [-0.76825466 -0.8462204 ]]



```python
# Printing an array of exponential values
print("Exponent of array elements:", np.exp(A))
```

    Exponent of array elements: [[6.83767123e+30 4.09399696e+35]
     [7.01673591e+20 9.74480345e+09]]



```python
# Printing square root of array values
print("Square root of array elements:", np.sqrt(A))
```

    Square root of array elements: [[8.42614977 9.05538514]
     [6.92820323 4.79583152]]

