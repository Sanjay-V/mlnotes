---
title: "Reversing words of a string"
author: "TACT"
date: 2019-04-20
description: "-"
type: technical_note
draft: false
---

```python
# Assigning a string value to the variable
input = 'New Delhi is the capital of India'
```


```python
# Split the string into words
data = input.split(' ')
```


```python
# Calling the reversed() built-in function to reverse the string
data = ' '.join(reversed(data))
```


```python
# Printing the reversed string
print(data)
```

    India of capital the is Delhi New

