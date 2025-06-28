# 扫码登录
## web端
### 申请二维码
API地址:`https://passport.bilibili.com/x/passport-login/web/qrcode/generate`  

#### 示例调用  
>URL


```
https://passport.bilibili.com/x/passport-login/web/qrcode/generate
```  
>python


```
import requests

print(requests.get(f"https://passport.bilibili.com/x/passport-login/web/qrcode/generate"))
```

#### 示例返回  
>json


```
{
  "code": 0,
  "message": "0",
  "ttl": 1,
  "data": {
    "url": "https://account.bilibili.com/h5/account-h5/auth/scan-web?navhide=1&callback=close&qrcode_key=d2ed5da2e9f3fc5d52064f18a2c85259&from=",
    "qrcode_key": "d2ed5da2e9f3fc5d52064f18a2c85259"
  }
}
```

#### 返回参数
| 参数地址  |  内容 |  示例 |  备注 |  
| ------------ | ---------------- | ------------ | ------------ |   
| .code  | 返回代码  | 0  |  0为正常(200) |  
|  .message | 错误代码  | 0  | 在code为0时此处也为0  |  
|  .ttl |  失效时间(s) | 1  | 二维码随时会过期,所以一般都是1  |  
| .data.url  | 二维码  | https://account.bilibili.com/h5/account-h5/auth/scan-web?navhide=1&callback=close&qrcode_key=d2ed5da2e9f3fc5d52064f18a2c85259&from= |  URL |  
| .data.qrcode_key  | 二维码key  | d2ed5da2e9f3fc5d52064f18a2c85259 |  和url中的qrcode_key参数一模一样 |  

#### 生成二维码
你可以使用python中的qrcode库来生成二维码,使用PIL以及tkinter库来显示二维码(tkinter库为官方标准库,无需安装)
##### 安装库
> cmd
```
pip install qrcode[pil]
```
##### 生成
> python
```
import qrcode

qr_url = # 返回中的.data.url

qr = qrcode.QRCode(
    version=1,
    error_correction=qrcode.constants.ERROR_CORRECT_L,
    box_size=10,
    border=4,
)
qr.add_data(qr_url)
qr.make(fit=True)

qc = qr.make_image(fill_color="black", back_color="white")
```
这样你就把生成的二维码保存到了qc变量
##### 显示
> python
```
from PIL import ImageTk,Image
import tkinter as tk

qc = # 刚刚生成的二维码
root = tk.Tk()

tk_image = ImageTk.PhotoImage(qc)

label = tk.Label(root, image=tk_image)
label.pack()

root.mainloop()
```
然后让用户扫码即可
#### 备注
生成的qrcode_key有效期为180秒

### 登录检查
API地址:`https://passport.bilibili.com/x/passport-login/web/qrcode/poll`
#### 参数  
| 参数名 | 类型   | 必填 | 说明               | 示例值           |
|--------|--------|------|--------------------|------------------|
| qrcode_key    | 字符串 | 是   | 二维码key     | d2ed5da2e9f3fc5d52064f18a2c85259 |

#### 示例调用  
>URL


```
https://passport.bilibili.com/x/passport-login/web/qrcode/poll?qrcode_key=d2ed5da2e9f3fc5d52064f18a2c85259
```  
>python


```
import requests

print(requests.get(f"https://passport.bilibili.com/x/passport-login/web/qrcode/poll?qrcode_key=d2ed5da2e9f3fc5d52064f18a2c85259"))
```

#### 示例返回  
>json


```
{
  "code": 0,
  "message": "0",
  "ttl": 1,
  "data": {
    "url": "",
    "refresh_token": "",
    "timestamp": 0,
    "code": 86101,
    "message": "未扫码"
  }
}
```

#### 返回参数
| 参数地址  |  内容 |  示例 |  备注 |  
| ------------ | ---------------- | ------------ | ------------ |   
| .code  | 返回代码  | 0  |  0为正常(200) |  
|  .message | 错误代码  | 0  | 在code为0时此处也为0  |  
|  .ttl |  失效时间(s) | 1  | 扫码状态随时会过期,所以一般都是1  |  
| .data.url  | 游戏分站跨域登录url  | (空) |  未登录为空 |  
| .data.refresh_token  | 刷新token  | (空) |  未登录为空 |  
| .data.timestamp | 登录时间 | 0 | 未登录为0,时间戳 |
| .data.code | 目前状态 | 86101 | 0:扫码登录成功<br>86038:二维码已失效<br>86090:二维码已扫码未确认<br>86101:未扫码<br>
| .data.message | 扫码状态 | 未扫码 | 无 |

## Github链接
[返回主页](https://qiufengcute.github.io/unofficial-bilibili-apis-docs/)  
[在Github上编辑此页(html)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/html/login.html)  
[在Github上编辑此页(markdown)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/markdown/login.md)  
[Github上的此项目](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/)
