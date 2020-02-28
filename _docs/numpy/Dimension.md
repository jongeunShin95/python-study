---
title: Dimension
category: numpy
order: 3
---

---
## 1. shape

(n행 x m열)을 보여준다.

* #### 6 x 1

```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6])
print(arr)
print(arr.shape)
```

    >>> [1 2 3 4 5 6]
    >>> (6, )

<br>

* #### 2 x 3

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])
print(arr)
print(arr.shape)
```

    >>> [[1 2 3]
         [4 5 6]]
    >>> (2, 3)

---

## 2. reshape()

리스트의 차원을 변경해준다.

* #### 6 x 1 -> 2 x 3

```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6]) # 6 x 1 리스트 생성
arr2 = arr.reshape(2, 3)
print(arr2)
print(arr.shape)
```

    >>> [[1 2 3]
         [4 5 6]]
    >>> (2, 3)

---

## 3. ndim

리스트의 차원을 보여준다.

* #### 1차원

```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6])
print(arr.ndim)
```

    >>> 1

<br>

* #### 2차원

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])
print(arr.ndim)
```

    >>> 2