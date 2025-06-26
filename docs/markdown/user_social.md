# 用户社交
API地址:https://api.bilibili.com/x/relation/stat

## 参数
|参数名|	类型	|必填|	说明|	示例值|
|---|---|---|---|---|
|vmid	|数字|	是|	查询用户的| UID|	3493083538786837|

## 示例调用
>URL


```
https://api.bilibili.com/x/relation/stat?vmid=3493083538786837
```


>python


```
import requests

print(requests.get(f"[https://api.bilibili.com/x/space/acc/info?mid=3493083538786837](https://api.bilibili.com/x/relation/stat?vmid=3493083538786837)"))
```


## 示例返回
>json


```
{
  "code": 0,
  "message": "0",
  "ttl": 1,
  "data": {
    "mid": 3493083538786837,
    "following": 400,
    "whisper": 0,
    "black": 0,
    "follower": 281
  }
}
```


## 返回参数
| 参数地址  |  内容 |  示例 |  备注 |  
| ------------ | ---------------- | ------------ | ------------ |   
| .code  | 返回代码  | 0  |  0为正常(200) |  
|  .message | 错误代码  | 0  | 在code为0是此处也为0  |  
|  .ttl |  失效时间(s) | 1  | 社交信息随时会变动,所以一般都是1  |  
| .data.mid | uid | 3493083538786837 | 无 |
| .data.following | 关注人数 | 400 | 无 |
| .data.whisper | 悄悄关注人数 | 0 | 目前悄悄关注已下线，所以基本上这里都是0 |
| .data.black | 黑名单人数 | 0 | 无 |
| .data.follower | 粉丝数 | 281 | 无 |

}
## Github链接
[返回主页](https://qiufengcute.github.io/unofficial-bilibili-apis-docs/)
[在Github上编辑此页(html)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/html/user_social.html)  
[在Github上编辑此页(markdown)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/markdown/user_social.md)  
[Github上的此项目](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/)

