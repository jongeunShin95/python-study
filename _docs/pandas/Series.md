---
title: Series
category: pandas
order: 2
---

---
## 1. Series()

데이터를 생성할 때 사용되는 함수이다.

* ### value값으로만 생성

```python
import pandas as pd

pd_data = pd.Series([1, 2, 3])
print(pd_data)
```

    >>> 0 1
        1 2
        2 3
        dtype: int64

* ### index값과 value값 주기

index값의 경우 정수뿐 아니라 문자도 가능하다.

```python
import pandas as pd

pd_data = pd.Series([1, 2, 3], [1, 2, 'a']) # 뒤 쪽이 index값이다.
print(pd_data)
```

    >>> 1 1
        2 2
        a 3