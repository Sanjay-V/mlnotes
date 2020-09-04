---
title: "Creating a Numpy Array"
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
# Creating a rank 1 Array and printing it out
arr = np.array([99, 47, 38])
print("Array with Rank 1: \n",arr)
```

    Array with Rank 1: 
     [99 47 38]



```python
# Creating a rank 2 Array and printing it out
arr = np.array([[11, 27, 35],
                [46, 52, 64]])
print("Array with Rank 2: \n", arr)
```

    Array with Rank 2: 
     [[11 27 35]
     [46 52 64]]



```python
# Creating an array from tuple and printing it out
arr = np.array((16, 34, 27))
print("\nArray created using "
      "passed tuple:\n", arr)
```

    
    Array created using passed tuple:
     [16 34 27]

