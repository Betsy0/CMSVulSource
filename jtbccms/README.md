### jtbccms

```
版本信息：3.0
```

#### 后台任意文件上传

登录后在联系我们处上传文件

![image-20221202143131775](images/image-20221202143131775.png)

然后抓包，将该请求包的URL修改

![image-20221202143222920](images/image-20221202143222920.png)

改为

```
/console/file/manage.php?type=action&action=addfile&path=../.././
```

![image-20221202143243875](images/image-20221202143243875.png)

上传后的文件

![image-20221202143422767](images/image-20221202143422767.png)

