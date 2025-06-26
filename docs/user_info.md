# 用户信息  
API地址：https://api.bilibili.com/x/space/acc/info 
## 参数  
|  参数名|  内容          |  示例    |  是否必填  |  备注  |
| ------| -------------- |----------|---------|---------|
|  mid  |  查询用户的uid  |  3493083538786837  |  是  |  无  |  

## 示例调用  
>URL


```
https://api.bilibili.com/x/space/acc/info?mid=3493083538786837
```  
>python


```
import requests

print(requests.get(f"https://api.bilibili.com/x/space/acc/info?mid=3493083538786837"))
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
    "name": "秋风wkhv",
    "sex": "男",
    "face": "https://i1.hdslb.com/bfs/face/a94fdc7eec613197f6a7f56232721f3940dc4812.jpg",
    "face_nft": 0,
    "face_nft_type": 0,
    "sign": "互关互助",
    "rank": 10000,
    "level": 5,
    "jointime": 0,
    "moral": 0,
    "silence": 0,
    "coins": 374.8,
    "fans_badge": false,
    "fans_medal": {
      "show": true,
      "wear": true,
      "medal": {
        "uid": 3493083538786837,
        "target_id": 431073645,
        "medal_id": 187507,
        "level": 12,
        "medal_name": "举爪爪",
        "medal_color": 9272486,
        "intimacy": 6149,
        "next_intimacy": 10000,
        "day_limit": 10000,
        "medal_color_start": 9272486,
        "medal_color_end": 9272486,
        "medal_color_border": 9272486,
        "is_lighted": 1,
        "light_status": 1,
        "wearing_status": 1,
        "score": 31050
      }
    },
    "official": {
      "role": 0,
      "title": "",
      "desc": "",
      "type": -1
    },
    "vip": {
      "type": 2,
      "status": 1,
      "due_date": 1759334400000,
      "vip_pay_type": 0,
      "theme_type": 0,
      "label": {
        "path": "http://i0.hdslb.com/bfs/vip/label_annual.png",
        "text": "年度大会员",
        "label_theme": "annual_vip",
        "text_color": "#FFFFFF",
        "bg_style": 1,
        "bg_color": "#FB7299",
        "border_color": "",
        "use_img_label": true,
        "img_label_uri_hans": "",
        "img_label_uri_hant": "",
        "img_label_uri_hans_static": "https://i0.hdslb.com/bfs/bangumi/kt/b52851866abcee9029b1bfb025d4a6ede3d461a6.png",
        "img_label_uri_hant_static": "https://i0.hdslb.com/bfs/activity-plat/static/20220614/e369244d0b14644f5e1a06431e22a4d5/VEW8fCC0hg.png",
        "label_id": 40,
        "label_goto": {
          "mobile": "",
          "pc_web": "https://account.bilibili.com/big?from_spmid=vipicon"
        }
      },
      "avatar_subscript": 1,
      "nickname_color": "#FB7299",
      "role": 3,
      "avatar_subscript_url": "",
      "tv_vip_status": 0,
      "tv_vip_pay_type": 0,
      "tv_due_date": 0,
      "avatar_icon": {
        "icon_type": 3,
        "icon_resource": {
          "type": 1,
          "url": "https://i0.hdslb.com/bfs/bangumi/kt/aba51485c0d02940c89aeefcf6680510d9858472.png"
        }
      }
    },
    "pendant": {
      "pid": 2701,
      "name": "七濑胡桃",
      "image": "https://i1.hdslb.com/bfs/garb/item/2c40fe802d1935d96e4fc63ec42274d8846a34b7.png",
      "expire": 0,
      "image_enhance": "https://i1.hdslb.com/bfs/garb/item/2c40fe802d1935d96e4fc63ec42274d8846a34b7.png",
      "image_enhance_frame": "",
      "n_pid": 2701
    },
    "nameplate": {
      "nid": 61,
      "name": "有爱楷模",
      "image": "https://i1.hdslb.com/bfs/face/5a90f715451325c642a6ac39e01195cb6d075734.png",
      "image_small": "https://i0.hdslb.com/bfs/face/5bfc1b4fb3f4b411495dddb0b2127ad80f6fbcac.png",
      "level": "普通勋章",
      "condition": "当前持有粉丝勋章最高等级\u003E=10级"
    },
    "user_honour_info": {
      "mid": 0,
      "colour": null,
      "tags": [],
      "is_latest_100honour": 0
    },
    "is_followed": false,
    "top_photo": "bfs/space/f35f1c09d709f5387814bbbfa614a391e73d9132.png",
    "sys_notice": {

    },
    "live_room": {
      "roomStatus": 1,
      "liveStatus": 0,
      "url": "https://live.bilibili.com/31826581?broadcast_type=0&is_room_feed=0",
      "title": "首次开播，请多关照！",
      "cover": "https://i0.hdslb.com/bfs/live/63a1e4a8fa91c2eac9321ce76b309b221c9be7a8.png",
      "roomid": 31826581,
      "roundStatus": 0,
      "broadcast_type": 0,
      "watched_show": {
        "switch": true,
        "num": 1,
        "text_small": "1",
        "text_large": "1人看过",
        "icon": "https://i0.hdslb.com/bfs/live/a725a9e61242ef44d764ac911691a7ce07f36c1d.png",
        "icon_location": "",
        "icon_web": "https://i0.hdslb.com/bfs/live/8d9d0f33ef8bf6f308742752d13dd0df731df19c.png"
      }
    },
    "birthday": "07-05",
    "school": {
      "name": ""
    },
    "profession": {
      "name": "",
      "department": "",
      "title": "",
      "is_show": 0
    },
    "tags": null,
    "series": {
      "user_upgrade_status": 3,
      "show_upgrade_window": false
    },
    "is_senior_member": 0,
    "mcn_info": null,
    "gaia_res_type": 0,
    "gaia_data": null,
    "is_risk": false,
    "elec": {
      "show_info": {
        "show": true,
        "state": 1,
        "title": "",
        "icon": "",
        "jump_url": "?oid=3493083538786837",
        "total": 2,
        "list": null
      }
    },
    "contract": {
      "is_display": false,
      "is_follow_display": false
    },
    "certificate_show": false,
    "name_render": null,
    "top_photo_v2": {
      "sid": 30495176,
      "l_img": "https://i0.hdslb.com/bfs/space/f35f1c09d709f5387814bbbfa614a391e73d9132.png",
      "l_200h_img": "https://i0.hdslb.com/bfs/space/f35f1c09d709f5387814bbbfa614a391e73d9132.png"
    },
    "theme": null,
    "attestation": {
      "type": 0,
      "common_info": {
        "title": "",
        "prefix": "",
        "prefix_title": ""
      },
      "splice_info": {
        "title": ""
      },
      "icon": "",
      "desc": ""
    }
  }
}
```

## 返回参数
| 参数地址  |  内容 |  示例 |  备注 |  
| ------------ | ------------ | ------------ | ------------ |   
| .code  | 返回代码  | 0  |  0为正常（200） |  
|  .message | 错误代码  | 0  | 在code为0是此处也为0  |  
|  .ttl |  失效时间（s） | 1  | 用户信息随时会变动，所以一般都是1  |  
| .data.mid  | uid  | 3493083538786837  |  无 |  
|  .data.name | 用户名  | 秋风wkhv  | 无  |   
| .data.sex  | 性别  |  男 |  无 |  
| .data.face  |  头像 | https://i1.hdslb.com/bfs/face/a94fdc7eec613197f6a7f56232721f3940dc4812.jpg  | URL  |  
| .data.face_nft  |  是否是数字藏品头像 |  0 | 0不是，1是  |  
| .data.face_nft_type  |  头像 NFT 类型 | 0  | 0应该是普通头像（非NFT），其他目前我不知道  |  
| .data.sign  | 个性签名  | 互关互助  | 无  |  
| .data.rank  |  用户等级标识 | 10000  | 我完全不知道  |  
|  .data.level | 等级  |  5 | 无  |  
| .data.jointime  | 入站时间（时间戳）  | 0  | 这个东西目前已经失效，之前是可以根据他获取入站时间的  |  
|  .data.moral |  道德分 |  0 | -n分  |  
|  .data.silence |  静言状态 |  0 | 0正常，1被禁言  |  
| .data.coins  |  硬币数量 | 374.8  | 小数是因为给视频投一个币=给up主0.1个币  |  
| .data.fans_badge  | 是否有粉丝勋章  | true  | true/false，即使过期也算  |  
| .data.fans_medal.show  | 是否显示粉丝勋章  | true  |  true/false |  
| .data.fans_medal.wear  |  是否佩戴勋章 | true  |  true/false |  
| .data.fans_medal.medal.uid  | 你的uid  | 3493083538786837  | 和.data.mid一模一样  |  
| .data.fans_medal.medal.target_id  |  主播的uid |  431073645 |  无 |  
| .data.fans_medal.medal.medal_id  |  勋章唯一ID | 187507  |  b站内部标识 |  
| .data.fans_medal.medal.level  | 勋章等级  | 12  |  无 |  
| .data.fans_medal.medal.medal_name  | 勋章名  | 举爪爪  |  无 |  
| .data.fans_medal.medal.medal_color  | 勋章主色  | 9272486  | RGB10进制值  |  
| .data.fans_medal.medal.next_intimacy  | 升级所需亲密度  | 10000  | 无  |  
| .data.fans_medal.medal.day_limit  | 一天最多可得亲密度  | 10000  | 无  |  
| .data.fans_medal.medal.medal_color_start  |  渐变起始色 | 9272486  | 同主色，无渐变时与主色一致  |  
| .data.fans_medal.medal.medal_color_end  |  渐变结束色 | 9272486  |  同主色 |  
| .data.fans_medal.medal.medal_color_border  | 边框颜色  | 9272486  | 同主色  |  
| .data.fans_medal.medal.is_lighted  |  是否点亮 | 1  |  短期过期还是1，但长期过期可能就变成0了 |  
| .data.fans_medal.medal.light_status  |  是否激活过 | 1  | 一般都是1（激活过），不会是0（没激活过），即使勋章已过期  |  
| .data.fans_medal.medal.wearing_status  |  佩戴状态 |  1 |  1=正在佩戴，0=未佩戴 |  
| .data.fans_medal.medal.score  | 总亲密度  |  31050 | 无  |  
| .data.official.role  |  认证角色类型 |  0 | 见附表1  |  
| .data.official.title  | 认证标题  |  （空） | 显示在用户主页的认证标识旁边的文字  |  
| .data.official.decs  | 认证描述  | （空）  | 对认证的详细说明  |  
| .data.official.type  | 认证大类  |  -1 | 见附表2  |  
| .data.vip.type  |  会员类型 |  2 |  0=无，1=月度，2=年度（含自动续费），3=其他 |  
| .data.vip.status  |  会员是否有效 |  1 | 0=过期，1=有效  |  
| .data.vip.due_date  | 到期时间  |  1759334400000 | 时间戳  |  
| .data.vip.vip_pay_type  | 支付方式  | 0  | 0=未付费（如活动赠送），1=已付费，2=自动续费开通（可能会有问题）  |  
| .data.vip.theme_type  | 主题样式  | 0  |  见附表3 |  
| .data.vip.label.path  | 会员图片  | http://i0.hdslb.com/bfs/vip/label_annual.png  | URL  |  
| .data.vip.label.text  | 会员名称  | 年度大会员  | 无  |  
| .data.vip.label.label_theme  | 标签主题样式标识  | annual_vip  |  此为年度大会员专属主题标识 |  
| .data.vip.label.text_color  |  文字颜色 | #FFFFFF  | 无  |  
| .data.vip.label.bg_style  |  背景样式类型  | 1  | 见附表4  |  
| .data.vip.label.bg_color | 标签背景色  | #FB7299 | 无 |  
| .data.vip.label.border_color  |  标签边框颜色  | （空）  | （空）=无边框  |  
| .data.vip.label.use_img_label | 是否使用图片标签  | true | true/false |  


## 附表

### 附表1  
| 值  |  含义 | 示例用户  |
| ------------ | ------------ | -------------|
| 0  |        无认证     |        普通用户  |
|  1 | 	官方认证（初级）  |小有名气的UP主|
|  2 | 知名认证（中级）| 头部UP主/主播 |
| 3  | 权威认证（高级）  |  明星/官方机构    |
|  4 | 用户名  | 企业认证    |	企业号|
|  5 | 用户名  |  政府/媒体认证  |政府机构/官媒|


### 附表2   
| 值  |  含义 |
| ------------ | ------------ |
| -1  |        无认证     |
|  0 | 	个人认证（普通UP主/主播）  |
|  1 | 机构认证（企业/学校等）|
| 2  | 政府/媒体认证  |


### 附表3   
| 值  |  含义 | 视觉效果 |
| ------------ | ------------ | --------- |
| 0  |   默认主题（无专属皮肤）   | 使用B站默认的蓝色/粉色主题|
|  1 | 	大会员基础主题  |轻度定制化配色（如浅金色点缀） |
|  2 | 年度大会员专属主题|高级动态皮肤（如节日限定、IP联名主题，示例：#FB7299 渐变 + 动态元素） |
| >2  | 特殊限定主题（需活动获取或付费）  |如「周年庆限定」「番剧联名」等稀有皮肤 |


### 附表3   
| 值  |  样式类型 | 视觉效果 |典型应用场景|
| ------------ | ------------ | --------- |----
| 0  |   无背景   | 仅显示文字（无背景色和边框）|简约模式/特殊活动
|  1 | 	纯色填充  |使用 bg_color 定义的单一颜色填充背景 |标准年度大会员标签
|  2 | 线性渐变|从 medal_color_start 到 medal_color_end 的横向渐变 |特殊活动限定标签
| 3  | 边框+填充  |带 border_color 定义的边框 + bg_color 填充 |高级会员或联名活动
| 4 |  动态流光  |  基础背景色 + 水平流动光效（需配合 use_img_label 使用）   |年度大会员促销期
| 5 |   径向渐变 |   从中心向四周的放射渐变（中心色 medal_color_start，边缘色 medal_color_end）  |限定IP合作主题


## 备注
这个API非常容易请求过于频繁
