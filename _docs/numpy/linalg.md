---
title: linalg
category: numpy
order: 7
---

---
## 1. linalg

* #### inv()
역행렬을 구해주는 함수이다.

```python
import numpy as np

arr = np.arange(1, 5).reshape(2, 2)

print(arr)
print(np.linalg.inv(arr))
```

    >>> [[1 2]
         [3 4]]
        [[-2. 1.]
         [1.5 -0.5]]

나온 행렬이 역행렬이 맞는지 확인하기 위해 주어진 행렬과 나온 역행렬을 곱하여 단위행렬이 나오는지 확인해본다.

```python
print(arr@np.linalg.inv(arr))
```

    >>> [[1.00000000e+00 1.11022302e-16]
         [0.00000000e+00 1.00000000e+00]]

나온 행렬을 보게 되면 완전한 0은 아니지만 0에 가까운 엄청 작은수이기 때문에 단위행렬이 나온 것을 확인 할 수 있다. 이 행렬이 단위 행렬인지 확인하기 위해 allclose()함수를 이용하여 비교해볼 수 있다.

```python
arr2 = np.array([[1, 0], [0, 1]])
print(arr2)
print(np.allclose(arr@np.linalg.inv(arr), arr2)) # 작은 오차 범위는 동등하다고 판단.
```

    >>> [[1 0]
         [0 1]]
        True

* #### solve()

다음과 같은 식을 풀기위해 사용된다.

```python
    x + y = 10
    2x + 3y = 25
```

```python
import numpy as np

arr1 = np.array([[1, 1], [2, 3]])
arr2 = np.array([10, 25])

answer = np.linalg.solve(arr1, arr2)
print(answer)
```

    >>> [5. 5.]