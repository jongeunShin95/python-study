---
title: mean, max, argmx
category: numpy
order: 4
---

---
## 1. mean()

리스트들의 평균을 나타낸다.

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr)
print(arr.mean())
```
    >>> [[1 2 3]
         [4 5 6]
         [7 8 9]]
        5.0

---

## 2. max()

리스트의 원소들 중 가장 큰 수를 반환한다.

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr)
print(np.max(arr))
```
    >>> [[1 2 3]
         [4 5 6]
         [7 8 9]]
        9

---

## 3. argmax()

리스트의 원소들 중 가장 큰 원소의 인덱스를 반환한다.

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr)
print(np.argmax(arr))
```

    >>> [[1 2 3]
         [4 5 6]
         [7 8 9]]
        8