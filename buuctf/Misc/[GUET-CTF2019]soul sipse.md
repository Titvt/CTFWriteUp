# [GUET-CTF2019]soul sipse

## 知识点

`steghide无密码分解`

`Unicode`

## 解题

![](./img/90-1.png)

没有什么有效信息,`binwalk`试试

![](./img/90-2.png)

![](./img/90-3.png)

`steghide`无密码分解出`download.txt`

```
https://share.weiyun.com/5wVTIN3
```

下载得到`GUET.png`，修改为正确的`PNG`文件头

![](./img/90-4.png)

保存得到正常的图片。如下

![](./img/90-5.png)

`Unicode`解码

![](./img/90-6.png)

```
 4070
+1234
------
 5304
```

```
flag{5304}
```

