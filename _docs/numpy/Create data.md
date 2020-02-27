---
title: Create data
category: numpy
order: 2
---

---
## 1. array()

#### 1차원
```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])
print(arr)
```
    >>> [1 2 3 4 5]

#### 2차원
```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])
print(arr)
```
    >>> [[1 2 3]
        [4 5 6]]
---
## 2. arrange()
#### 1개의 인자값
```python
import numpy as np

arr = np.arange(5)
print(arr)
```
    >>> [0 1 2 3 4]
#### 2개의 인자값
```python
import numpy as np

arr = np.arange(1, 6)
print(arr)
```
    >>> [1 2 3 4 5]
#### 3개의 인자값
```python
import numpy as np

arr = np.arange(1, 10, 2)
print(arr)
```
    >>> [1 3 5 7 9]
---
## 3. ones(), zeros()
#### ones()
```python
import numpy as np

arr = ones((2, 2))
print(arr)
```
    >>> [[1. 1.]
         [1. 1.]]
#### zeros()
```python
import numpy as np

arr = ones((2, 2))
print(arr)
```
    >>> [[0. 0.]
         [0. 0.]]