

使用sklearn库中的KMeans算法对数据进行分群

![image](https://github.com/funnymax/blog/assets/111578882/328a865b-a5e0-4225-a53e-b3aebd331550)

```python
import pandas as pd
from sklearn.cluster import KMeans
d = xl("C5:DH492", headers=False) #此处引用特征数据，不含表头
d = d.fillna(value=0)
kmeans = KMeans(n_clusters=8)
output = kmeans.fit_predict(d)
list(output)
```
