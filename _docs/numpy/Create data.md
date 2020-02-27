---
title: Create data
category: numpy
order: 2
---

---
## array()

* #### 1차원

```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])
print(arr)
```
    >>> [1 2 3 4 5]

<br>

* #### 2차원

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])
print(arr)
```
    >>> [[1 2 3]
        [4 5 6]]

---

## arrange()

* #### 1개의 인자값

```python
import numpy as np

arr = np.arange(5)
print(arr)
```
    >>> [0 1 2 3 4]

<br>

* #### 2개의 인자값

```python
import numpy as np

arr = np.arange(1, 6)
print(arr)
```
    >>> [1 2 3 4 5]

<br>

* #### 3개의 인자값

```python
import numpy as np

arr = np.arange(1, 10, 2)
print(arr)
```
    >>> [1 3 5 7 9]

---
## ones(), zeros()

* #### ones()

```python
import numpy as np

arr = ones((2, 2))
print(arr)
```
    >>> [[1. 1.]
         [1. 1.]]

<br>

* #### zeros()

```python
import numpy as np

arr = ones((2, 2))
print(arr)
```
    >>> [[0. 0.]
         [0. 0.]]