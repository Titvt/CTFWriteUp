# [MRCTF2020]小O的考研复试

## 知识点

`数学计算`

## 解题

![](./img/106-1.png)

```python
a=2
for i in range(19260816):
    a = a * 10 + 2
    a%=(1e9+7)

print(a)
```

`577302567`