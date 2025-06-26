# 公告  
API地址:https://api.bilibili.com/x/space/notice
## 参数  
| 参数名 | 类型   | 必填 | 说明               | 示例值           |
|--------|--------|------|--------------------|------------------|
| mid    | number | 是   | 查询用户的 UID     | 3493083538786837 |

## 示例调用  
>URL


```
https://api.bilibili.com/x/space/notice?mid=3493083538786837
```  
>python


```
import requests

print(requests.get(f"https://api.bilibili.com/x/space/notice?mid=3493083538786837"))
```

## 示例返回  
>json


```
{
  "code": 0,
  "message": "0",
  "ttl": 1,
  "data": ""
}
```

## 返回参数
| 参数地址  |  内容 |  示例 |  备注 |  
| ------------ | ---------------- | ------------ | ------------ |   
| .code  | 返回代码  | 0  |  0为正常(200) |  
|  .message | 错误代码  | 0  | 在code为0是此处也为0  |  
|  .ttl |  失效时间(s) | 1  | 公告随时会变动,所以一般都是1  |  
| .data  | 公告内容  | (空) |  空是因为我没有公告 |  

## Github链接
[在Github上编辑此页(html)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/html/notice.html)  
[在Github上编辑此页(markdown)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/markdown/notice.md)  
[Github上的此项目](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/)
