---
title: "Swapping First and Last Elements of a list"
author: "TACT"
date: 2019-04-20
description: "-"
type: technical_note
draft: false
---

```python
# Assigning Swap function 
def swap(new): 
    new[0], new[-1] = new[-1], new[0] 
    return new
```


```python
# Assigning value for swap function
new = [23, 36, 90, 57, 64] 
```


```python
# Calling swap function
value = (swap(new)) 
print("New list will be ", value) 
```

    New list will be  [64, 36, 90, 57, 23]

