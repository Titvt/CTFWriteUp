# [DDCTF2018]第四扩展FS

## 知识点

`foremost分离`

`频次统计`

## 解题

得到一张`jpg`

![](./img/116-1.png)

详细信息里面有内容

![](./img/116-2.png)

`foremost`分离一下

![](./img/116-3.png)

根据详细信息中的备注作为密码,解压出一个文件

![](./img/116-4.png)

频次统计

```python
from collections import Counter

with open('./file.txt', 'r') as f:
    cont = f.read()
    res = Counter(cont)
    print(''.join(res.keys()))
```

![](./img/116-5.png)

组合一下即可