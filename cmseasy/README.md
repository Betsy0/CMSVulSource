### cmseasy

```
版本信息：7.6.3.2
```

#### 支付逻辑漏洞

首先注册一个账户，可以看到账户是0元

![Snipaste_2022-10-28_13-57-39.jpg](images/Snipaste_2022-10-28_13-57-39.jpg)

然后在精选产品里随意选择一个商品购买

![Snipaste_2022-10-28_14-07-30.jpg](images/Snipaste_2022-10-28_14-07-30.jpg)

然后抓包

![Snipaste_2022-10-28_14-07-47.jpg](images/Snipaste_2022-10-28_14-07-47.jpg)

将thisnum的值修改为负数，可以看到金额变成了负数

![Snipaste_2022-10-28_14-08-07.jpg](images/Snipaste_2022-10-28_14-08-07.jpg)

进入到支付页面选择余额支付

![Snipaste_2022-10-28_14-08-39.jpg](images/Snipaste_2022-10-28_14-08-39.jpg)

可以看到购买成功

![Snipaste_2022-10-28_14-08-52.jpg](images/Snipaste_2022-10-28_14-08-52.jpg)

回到个人中心了也可以看到自己的余额变多了

![Snipaste_2022-10-28_14-09-18.jpg](images/Snipaste_2022-10-28_14-09-18.jpg)





