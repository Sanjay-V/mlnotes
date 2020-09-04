---
title: "Reversing a list"
author: "TACT"
date: 2019-04-20
description: "-"
type: technical_note
draft: false
---

```python
# Reversing a list using reverse() assigned in a function
def Reverse(lst): 
    lst.reverse() 
    return lst 
```


```python
# Assigning values to list
lst = [10, 11, 12, 13, 14, 15] 
```


```python
# Printing the Reversed list
print(Reverse(lst))
```

    [15, 14, 13, 12, 11, 10]

