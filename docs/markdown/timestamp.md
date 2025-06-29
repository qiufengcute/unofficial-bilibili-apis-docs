# 时间戳
## 获取当前时间戳
第一类
API地址:`https://api.bilibili.com/x/report/click/now`

### 示例调用  
>URL


```
https://api.bilibili.com/x/report/click/now
```  
>python


```
import requests

print(requests.get(f"https://api.bilibili.com/x/report/click/now"))
```

### 示例返回  
>json


```
{
  "code": 0,
  "message": "0",
  "ttl": 1,
  "data": {
    "now": 1751172273
  }
}
```

### 返回参数
| 参数地址  |  内容 |  示例 |  备注 |  
| ------------ | ---------------- | ------------ | ------------ |   
| .code  | 返回代码  | 0  |  0为正常(200) |  
|  .message | 错误代码  | 0  | 在code为0时此处也为0  |  
|  .ttl |  失效时间(s) | 1  | 时间戳随时会变动,所以一般都是1  |  
| .data.now  | 当前时间戳  | 1751172273 |  无 |  
## 获取适用于 RTC 的时间戳
第一类  
API地址:`https://api.live.bilibili.com/xlive/open-interface/v1/rtc/getTimestamp`

### 示例调用  
>URL


```
https://api.live.bilibili.com/xlive/open-interface/v1/rtc/getTimestamp
```  
>python


```
import requests

print(requests.get(f"https://api.live.bilibili.com/xlive/open-interface/v1/rtc/getTimestamp"))
```
### 示例返回  
>json


```
{
  "code": 0,
  "message": "0",
  "ttl": 1,
  "data": {
    "timestamp": 1751172575,
    "microtime": 1751172575378
  }
}
```

### 返回参数
| 参数地址  |  内容 |  示例 |  备注 |  
| ------------ | ---------------- | ------------ | ------------ |   
| .code  | 返回代码  | 0  |  0为正常(200) |  
|  .message | 错误代码  | 0  | 在code为0时此处也为0  |  
|  .ttl |  失效时间(s) | 1  | 时间戳随时会变动,所以一般都是1  |  
| .data.timestamp  | 服务器端UTC时间戳  | 1751172273 |  和"获取当前时间戳"那边获取出来的json中的.data.now一模一样 |  
| .data.microtime  | 服务器端UTC时间戳  | 1751172575378 |  毫秒级 |  

## Github链接
[返回主页](https://qiufengcute.github.io/unofficial-bilibili-apis-docs/)  
[在Github上编辑此页(html)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/html/timestamp.html)  
[在Github上编辑此页(markdown)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/markdown/timestamp.md)  
[Github上的此项目](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/)
