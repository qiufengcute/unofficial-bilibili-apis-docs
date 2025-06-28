# 用户互动  
第一类
API地址:`https://api.bilibili.com/x/space/upstat`  
## 参数  
| 参数名 | 类型   | 必填 | 说明               | 示例值           |
|--------|--------|------|--------------------|------------------|
| mid    | 数字 | 是   | 查询用户的 UID     | 3493083538786837 |

## 示例调用  
>URL


```
https://api.bilibili.com/x/space/upstat?mid=3493083538786837?mid=3493083538786837
```  
>python


```
import requests

print(requests.get(f"https://api.bilibili.com/x/space/upstat?mid=3493083538786837?mid=3493083538786837"))
```

## 示例返回  
>json


```
{
  "code": 0,
  "message": "0",
  "ttl": 1,
  "data": {
    "archive": {
      "enable_vt": 0,
      "view": 14736,
      "vt": 0
    },
    "article": {
      "view": 0
    },
    "likes": 360
  }
}
```

## 返回参数
| 参数地址  |  内容 |  示例 |  备注 |  
| ------------ | ---------------- | ------------ | ------------ |   
| .code  | 返回代码  | 0  |  0为正常(200) |  
|  .message | 错误代码  | 0  | 在code为0时此处也为0  |  
|  .ttl |  失效时间(s) | 1  | 互动信息随时会变动,所以一般都是1  |  
| .data.archive.enable_vt  | VT功能启用状态  | 0 |  0=未启用(VT可能是某种互动功能) |  
| .data.archive.view | 视频总播放量 | 14736 | 无 |
| .data.archive.vt | VT相关数据值 | 0 | 具体含义不明，当前为0 |
| .data.article.view | 文章总阅读量 | 0 | 无 |
| .data.likes | 获得的总点赞数 | 360 | 无 |


## Github链接
[返回主页](https://qiufengcute.github.io/unofficial-bilibili-apis-docs/)  
[在Github上编辑此页(html)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/html/user_Interactions.html)  
[在Github上编辑此页(markdown)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/markdown/user_Interactions.md)  
[Github上的此项目](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/)
