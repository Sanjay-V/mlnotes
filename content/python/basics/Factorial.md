---
title: "Factorial"
author: "TACT"
date: 2019-04-20
description: "-"
type: technical_note
draft: false
---

```python
# Assigning factorial function
def factorial(n): 
    if n < 0: 
        return 0
    elif n == 0 or n == 1: 
        return 1
    else: 
        fact = 1
        while(n > 1): 
            fact *= n 
            n -= 1
        return fact 
```


```python
# Assigning value for factorial function
num = 3
```


```python
# Calling factorial function
fact =  factorial(num)
print("Factorial of", num, "is", fact) 
```

    Factorial of 3 is 6

