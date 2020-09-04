---
title: "Accuracy Score"
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
# Importing Accuracy Score metric from sklearn
from sklearn.metrics import accuracy_score
```


```python
# Identifying accuracy_score and printing it out
score = accuracy_score(y_true, y_pred)    
print(score)
```

    0.8333333333333334



```python
# Returns the number of correctly classified samples
score = accuracy_score(y_true, y_pred, normalize=False)
print(score)
```

    5

