# unofficial-bilibili-apis-docs(简称UBAD)
<h3 align="center">
  <a href="https://qiufengcute.github.io/unofficial-bilibili-apis-docs/" style="display: inline-block;">
    <img src="img/icon.png" width="100" alt="UBAD">
  </a>
</h3>

[![GitHub stars](https://img.shields.io/github/stars/qiufengcute/unofficial-bilibili-apis-docs.svg?style=flat&color=yellow)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/stargazers)
[![GitHub license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/blob/master/LICENSE)
[![我的b站账号](img/bilibili.png)](https://space.bilibili.com/3493083538786837)  
一个不经常更新的非官方b站API文档  
我的b站uid是3493083538786837,后续将会经常出现  

>**⚠️警告**  
>请勿滥用,本项目仅用于学习!


## 目录  
> [json获取键](decs/html/get_json_text.html)


- [用户信息](docs/html/user_info.html)  
- [公告](docs/html/notice.html)
- [用户社交](docs/html/user_social.html)
- [用户创作](docs/html/user_authoring.html)
- [用户互动](docs/html/user_Interactions.html)
- [扫码登录](docs/html/login.html)
- [修改个性签名](docs/html/edit_sign.html)
- [时间戳](docs/html/timestamp.html)

## 备注
本项目中的所有API链接将分2大类:  
第一类:获取信息类 需要使用Get进行请求  
第二类:修改信息类 需要使用Post进行请求  

## 头部及cookies
最近,b站API好像变严格了  
如果不加头部及cookies就会出现412错误  
所以我提供一些信息  

### 头部
```
{
    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Safari/537.36",
    "Referer": "https://www.bilibili.com/",
    "Origin": "https://www.bilibili.com"
}
```

### cookies
```
{
    "SESSDATA": "见下文",
    "bili_jct": "见下文"
}
```

#### SESSDATA获取方式:
```
打开bilibili.com(请使用浏览器打开!!!),登录账号
点击F12(或者右键任意位置,点击检查)
点击"应用程序"
点击Cookie中的"https://www.bilibili.com"
点击SESSDATA
就是这里面的值
```

#### bili_jct获取方式:
```
打开bilibili.com(请使用浏览器打开!!!),登录账号
点击F12(或者右键任意位置,点击检查)
点击"应用程序"
点击Cookie中的"https://www.bilibili.com"
点击bili_jct
就是这里面的值
```

## Github链接
[在Github上编辑此页(html)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/index.html)  
[在Github上编辑此页](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/README.md)  
[GithubSE上的此项目](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/)
