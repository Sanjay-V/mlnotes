---
title: "Array Characteristics"
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
# Printing type of arr object
print("Array is of type: ", type(arr))
```

    Array is of type:  <class 'numpy.ndarray'>



```python
# Printing array dimensions (axes)
print("No. of dimensions: ", arr.ndim)
```

    No. of dimensions:  2



```python
# Printing shape of array
print("Shape of array: ", arr.shape)
```

    Shape of array:  (2, 3)



```python
# Printing size (total number of elements) of array
print("Size of array: ", arr.size)
```

    Size of array:  6



```python
# Printing type of elements in array
print("Array stores elements of type: ", arr.dtype)
```

    Array stores elements of type:  int64

