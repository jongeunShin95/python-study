---
title: Series Basic Func
category: pandas
order: 3
---

---
## 1. dataset

예제들을 위한 데이터 생성

* ### dataset
```python
import pandas as pd
import numpy as np

pd_data = pd.Series([1, 1, 2, 3, np.NAN])
print(pd_data)
```

    >>> 0 1.0
        1 1.0
        2 2.0
        3 3.0
        4 NaN
        dtype: float64

---

## 2. size

데이터의 갯수를 반환한다.

```python
print(pd_data.size)
```

    >>> 5

### 3. shape

몇과 열을 반환한다.

```python
print(pd_data.shape)
```

    >>> (5,)

### 4. unique()

중복되는 값은 빼고 반환다.

```python
print(pd_data.unique())
```

    >>> array([1., 2., 3., nan])

### 5. mean()

numpy와는 다르게 NaN값이 존재해도 그 값은 빼고 평균을 구해준다.

```python
print(pd_data.mean())
```

    >>> 1.75


### head, tail

각각 상위, 하위 5개의 데이터를 출력해준다. 나중에 많은 데이터들을 다룰 때 데이터들이 제대로 들어갔는지 확인하기 위해 사용된다. 인자값으로 갯수를 넘겨주면 해당 갯수만큼 출력된다.