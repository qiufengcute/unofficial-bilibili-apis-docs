# 用户创作
API地址:`https://api.bilibili.com/x/space/navnum`

## 参数
|参数名|	类型	|必填|	说明|	示例值|
|---|---|---|---|---|
|mid	|数字|	是|	查询用户的UID|	3493083538786837|

## 示例调用
>URL


```
https://api.bilibili.com/x/space/navnum?mid=3493083538786837
```


>python


```
import requests

print(requests.get(f"https://api.bilibili.com/x/space/navnum?mid=3493083538786837"))
```


## 示例返回
>json


```
{
  "code": 0,
  "message": "0",
  "ttl": 1,
  "data": {
    "video": 52,
    "bangumi": 0,
    "cinema": 1,
    "channel": {
      "master": 2,
      "guest": 2
    },
    "favourite": {
      "master": 7,
      "guest": 7
    },
    "tag": 0,
    "article": 0,
    "playlist": 0,
    "album": 5,
    "audio": 0,
    "pugv": 0,
    "season_num": 1,
    "opus": 5
  }
}
```


## 返回参数
| 参数地址  |  内容 |  示例 |  备注 |  
| ------------ | ---------------- | ------------ | ------------ |   
| .code  | 返回代码  | 0  |  0为正常(200) |  
|  .message | 错误代码  | 0  | 在code为0时此处也为0  |  
|  .ttl |  失效时间(s) | 1  | 创作信息随时会变动,所以一般都是1  |  
| .data.video | 上传视频数 | 52 | 无 |
| .data.bangumi | 上传的番剧/国创动画数 | 0 | 无 |
| .data.cinema | 影视内容数 | 1 | 无 |
| .data.channel.master | 主频道数 | 2 | 无 |
| .data.channel.guest | 参与频道数 | 0 | 无 |
| .data.favourite.master | 创建收藏夹数 | 7 | 无 |
| .data.favourite.guest | 参与收藏夹数 | 7 | 无 |
| .data.tag | 创建的标签数 | 0 | 无 |
| .data.article | 发布的专栏文章数 | 0 | 无 |
| .data.playlist | 创建的播单/视频合集数 | 0 | 无 |
| .data.album | 相册数 | 5 | 无 |
| .data.audio | 上传的音频数 | 0 | 无 |
| .data.pugv | 参与的PUGV课程数 | 0 | PUGV=专业用户生成视频 |
| .data.season_num | 合集/系列数 | 1 | 无 |
| .data.opus | 动态/作品数 | 5 | 无 |

## Github链接
[返回主页](https://qiufengcute.github.io/unofficial-bilibili-apis-docs/)  
[在Github上编辑此页(html)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/html/user_authoring.html)  
[在Github上编辑此页(markdown)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/markdown/user_authoring.md)  
[Github上的此项目](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/)
