---
title: "Joining the string"
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
# Split the string into words by calling split() built-in function
data = input.split(' ')
```


```python
# Print the splitted string
print(data)
```

    ['New', 'Delhi', 'is', 'the', 'capital', 'of', 'India']



```python
# Join the string by calling join() built-in function
string = '-'.join(data)
```


```python
# Print the joined string
print(string)
```

    New-Delhi-is-the-capital-of-India

