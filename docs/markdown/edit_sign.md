# 编辑个性签名 
第二类  
API地址:`https://api.bilibili.com/x/member/web/sign/update`  

## 参数  
| 参数名 | 类型   | 必填 | 说明               | 示例值           |
|--------|--------|------|--------------------|------------------|
| access_key    | 字符串 | 与csrf二选一   | APP登录Token     | (保密) |
| csrf    | 字符串 | 与access_key二选一   | Token(位于cookie)     | (保密) |
| user_sign    | 字符串 | 否   | 要设置的签名内容     | 互关互助\|个人博客:https://www.yuque.com/qiufengqiufeng-qxav8/fgoums |

## 示例调用  
>URL


```
https://api.bilibili.com/x/member/web/sign/update?csrf=***&user_sign=互关互助|个人博客:https://www.yuque.com/qiufengqiufeng-qxav8/fgoums
```  
>python


```
import requests

print(requests.get(f"https://api.bilibili.com/x/member/web/sign/update?csrf=***&user_sign=互关互助|个人博客:https://www.yuque.com/qiufengqiufeng-qxav8/fgoums"))
```

## 示例返回  
>json


```
{
  "code":0,
  "message":"0",
  "ttl":1
}
```

## 返回参数
| 参数地址  |  内容 |  示例 |  备注 |  
| ------------ | ---------------- | ------------ | ------------ |   
| .code  | 返回代码  | 0  |  0为正常(200) |  
|  .message | 错误代码  | 0  | 在code为0时此处也为0  |  
|  .ttl |  失效时间(s) | 1  | 我不知道怎么解释了  |  

## 备注
csrf为cookie中的bili_jct  
需要额外添加SESSDATA(也在cookie中)  
修改签名不会立即生效,会等待审核队列稍后生效(审核还挺快的)  
签名最多支持70个字符

## Github链接
[返回主页](https://qiufengcute.github.io/unofficial-bilibili-apis-docs/)  
[在Github上编辑此页(html)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/html/edit_sign.html)  
[在Github上编辑此页(markdown)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/markdown/edit_sign.md)  
[Github上的此项目](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/)
