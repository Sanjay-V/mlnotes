---
title: "Confusion Matrix"
author: "Sanjay"
date: 2020-09-04
description: "-"
type: technical_note
draft: false
---

```python
# Import Numpy library  
import numpy as np
```


```python
# Initialize list values
y_pred = [0, 2, 0, 2, 1,3]
y_true = [0, 2, 3, 2, 1,3]
```


```python
# Importing confusion_matrix metric from sklearn
from sklearn.metrics import confusion_matrix
```


```python
# Printing out the confusion matrix
matrix = confusion_matrix(y_true, y_pred)    
print(matrix)
```

    [[1 0 0 0]
     [0 1 0 0]
     [0 0 2 0]
     [1 0 0 1]]

