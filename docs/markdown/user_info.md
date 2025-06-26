# 用户信息  
API地址:https://api.bilibili.com/x/space/acc/info 
## 参数  
| 参数名 | 类型   | 必填 | 说明               | 示例值           |
|--------|--------|------|--------------------|------------------|
| mid    | number | 是   | 查询用户的 UID     | 3493083538786837 |

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
| ------------ | ---------------- | ------------ | ------------ |   
| .code  | 返回代码  | 0  |  0为正常(200) |  
|  .message | 错误代码  | 0  | 在code为0是此处也为0  |  
|  .ttl |  失效时间(s) | 1  | 用户信息随时会变动,所以一般都是1  |  
| .data.mid  | uid  | 3493083538786837  |  无 |  
|  .data.name | 用户名  | 秋风wkhv  | 无  |   
| .data.sex  | 性别  |  男 |  无 |  
| .data.face  |  头像 | https://i1.hdslb.com/bfs/face/a94fdc7eec613197f6a7f56232721f3940dc4812.jpg  | URL  |  
| .data.face_nft  |  是否是数字藏品头像 |  0 | 0不是,1是  |  
| .data.face_nft_type  |  头像 NFT 类型 | 0  | 0应该是普通头像(非NFT),其他目前我不知道  |  
| .data.sign  | 个性签名  | 互关互助  | 无  |  
| .data.rank  |  用户等级标识 | 10000  | 我完全不知道  |  
|  .data.level | 等级  |  5 | 无  |  
| .data.jointime  | 入站时间(时间戳)  | 0  | 这个东西目前已经失效,之前是可以根据他获取入站时间的  |  
|  .data.moral |  道德分 |  0 | -n分  |  
|  .data.silence |  静言状态 |  0 | 0正常,1被禁言  |  
| .data.coins  |  硬币数量 | 374.8  | 小数是因为给视频投一个币=给up主0.1个币  |  
| .data.fans_badge  | 是否有粉丝勋章  | true  | true/false,即使过期也算  |  
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
| .data.fans_medal.medal.medal_color_start  |  渐变起始色 | 9272486  | 同主色,无渐变时与主色一致  |  
| .data.fans_medal.medal.medal_color_end  |  渐变结束色 | 9272486  |  同主色 |  
| .data.fans_medal.medal.medal_color_border  | 边框颜色  | 9272486  | 同主色  |  
| .data.fans_medal.medal.is_lighted  |  是否点亮 | 1  |  短期过期还是1,但长期过期可能就变成0了 |  
| .data.fans_medal.medal.light_status  |  是否激活过 | 1  | 一般都是1(激活过),不会是0(没激活过),即使勋章已过期  |  
| .data.fans_medal.medal.wearing_status  |  佩戴状态 |  1 |  1=正在佩戴,0=未佩戴 |  
| .data.fans_medal.medal.score  | 总亲密度  |  31050 | 无  |  
| .data.official.role  |  认证角色类型 |  0 | 见附表1  |  
| .data.official.title  | 认证标题  |  (空) | 显示在用户主页的认证标识旁边的文字  |  
| .data.official.decs  | 认证描述  | (空)  | 对认证的详细说明  |  
| .data.official.type  | 认证大类  |  -1 | 见附表2  |  
| .data.vip.type  |  会员类型 |  2 |  0=无,1=月度,2=年度(含自动续费),3=其他 |  
| .data.vip.status  |  会员是否有效 |  1 | 0=过期,1=有效  |  
| .data.vip.due_date  | 到期时间  |  1759334400000 | 时间戳  |  
| .data.vip.vip_pay_type  | 支付方式  | 0  | 0=未付费(如活动赠送),1=已付费(可能会有问题)  |  
| .data.vip.theme_type  | 主题样式  | 0  |  见附表3 |  
| .data.vip.label.path  | 会员图片  | http://i0.hdslb.com/bfs/vip/label_annual.png  | URL  |  
| .data.vip.label.text  | 会员名称  | 年度大会员  | 无  |  
| .data.vip.label.label_theme  | 标签主题样式标识  | annual_vip  |  此为年度大会员专属主题标识 |  
| .data.vip.label.text_color  |  文字颜色 | #FFFFFF  | 无  |  
| .data.vip.label.bg_style  |  背景样式类型  | 1  | 见附表4  |  
| .data.vip.label.bg_color | 标签背景色  | #FB7299 | 无 |  
| .data.vip.label.border_color  |  标签边框颜色  | (空)  | (空)=无边框  |  
| .data.vip.label.use_img_label | 是否使用图片标签  | true | true/false |  
| .data.vip.label.img_label_uri_hans | 简体中文动态标签图片(未启用时为空)  | (空) | URL |  
| .data.vip.label.img_label_uri_hant  |  繁体中文动态标签图片(未启用时为空)  | (空)  | URL  |  
| .data.vip.label.img_label_uri_hans_static | 简体中文静态标签图片 | https://i0.hdslb.com/bfs/bangumi/kt/b52851866abcee9029b1bfb025d4a6ede3d461a6.png | URL,实际显示的图片 | 
| .data.vip.label.img_label_uri_hant_static | 繁体中文静态标签图片 | https://i0.hdslb.com/bfs/activity-plat/static/20220614/e369244d0b14644f5e1a06431e22a4d5/VEW8fCC0hg.png | URL,实际显示的图片 |
| .data.vip.label.label_id | 大会员标签类型ID | 40 | 10=月度大会员,20=季度大会员,40=年度大会员 |
| .data.vip.label.label_goto.mobile | 移动端点击标签跳转URL | (空) | 留空表示使用默认行为 |
| .data.vip.label.label_goto.pc_web | PC端点击标签跳转URL | https://account.bilibili.com/big?from_spmid=vipicon | 通常指向大会员权益页 |
| .data.vip.avatar_subscript | 头像角标显示控制 | 1 | 0=不显示,1=显示 |
| .data.vip.nickname_color | 昵称专属颜色 | #FB7299 | 无 |
| .data.vip.role | 会员权限等级 | 3 | 1=普通大会员,3=年度/高级大会员 |
| .data.vip.avatar_subscript_url | 预留字段(始终为空) | (空) | 未来可能用于动态角标 |
| .data.vip.tv_vip_status | 电视端VIP状态 | 0 | 0=未开通,1=有效 |
| .data.vip.tv_vip_pay_type | 电视端支付方式 | 0 | 0=未付费(如活动赠送),1=已付费(可能会有问题) |
| .data.vip.tv_due_date | 电视端VIP到期时间戳 | 0 | 0表示未开通 |
| .data.vip.avatar_icon.icon_type | 角标类型 | 3 | 见附表5 |
| .data.vip.avatar_icon.icon_resource.type | 资源类型 | 1 | 见附表6 |
| .data.vip.avatar_icon.icon_resource.url | 角标图片地址 | https://i0.hdslb.com/bfs/bangumi/kt/aba51485c0d02940c89aeefcf6680510d9858472.png | 无 |
| .data.pendant.pid | 挂件唯一ID | 2701 | 无 |
| .data.pendant.name | 挂件显示名称 | 七濑胡桃 | 无 |
| .data.pendant.image | 标准版挂件图片 | https://i1.hdslb.com/bfs/garb/item/2c40fe802d1935d96e4fc63ec42274d8846a34b7.png | URL,分辨率较低,已逐渐弃用 |
| .data.pendant.expire | 挂件过期时间 | 0 | 0=永久有效,时间戳 |
| .data.pendant.image_enhance | 高清版挂件图片 | https://i1.hdslb.com/bfs/garb/item/2c40fe802d1935d96e4fc63ec42274d8846a34b7.png | URL,当前实际使用的资源|
| .data.pendant.image_enhance_frame | 动态挂件的边框特效资源 | (空) | URL,空表示静态挂件
| .data.pendant.n_pid | 新版挂件唯一ID | 2701 | 与旧版相同时表示未更新 |
| .data.nameplate.nid | 勋章唯一ID | 61 | 无 |
| .data.nameplate.name | 勋章名称 | 有爱楷模 | 无 |
| .data.nameplate.image | 标准尺寸勋章图片 | https://i1.hdslb.com/bfs/face/5a90f715451325c642a6ac39e01195cb6d075734.png | URL,约100×100px |
| .data.nameplate.image_small | 小尺寸勋章图片 | https://i0.hdslb.com/bfs/face/5bfc1b4fb3f4b411495dddb0b2127ad80f6fbcac.png | URL,约50×50px,用于评论区等小空间展示 |
| .data.nameplate.level | 勋章等级分类 | 普通勋章 | 普通/稀有/限定 |
| .data.nameplate.condition | 获取条件说明 | 当前持有粉丝勋章最高等级\u003E=10级 | 含Unicode转义字符\u003E表示>符号,大部分语言在读取json时会把它转换回去 |
| .data.user_honour_info.mid | 预留字段 | 0 | 始终为0 |
| .data.user_honour_info.colour | 荣誉标签颜色值 | null | RGB HEX,为null表示无荣誉|
| .data.user_honour_info.tags | 荣誉标签列表 | [] | 空数组表示当前无荣誉|
| .data.user_honour_info.is_latest_100honour | 是否进入 高能100 榜单 | 0 | 0=未进入,1=已进入|
| .data.is_followed | 当前查询者是否已关注被查询者 | false | 需要登录态,未登录或查询自己时固定返回false |
| .data.top_photo | 个人主页顶部横幅图 | bfs/space/f35f1c09d709f5387814bbbfa614a391e73d9132.png | 完整URL=https://i0.hdslb.com/+top_photo |
| .data.sys_notice | 预留字段 | {} | 曾用于封禁通知等系统消息(现改用独立API),目前始终为空对象{} |
| .data.live_room.roomStatus | 直播间开通状态 | 1 | 0=未开通,1=已开通 |
| .data.live_room.liveStatus | 直播状态 | 0 | 0=未开播,1/2=直播中 |
| .data.live_room.url | 直播间完整URL | https://live.bilibili.com/31826581?broadcast_type=0&is_room_feed=0 | 含跟踪参数 |
| .data.live_room.title | 直播间标题 | 首次开播，请多关照！ | 最后一场直播的标题 |
| .data.live_room.cover | 直播间封面图 | https://i0.hdslb.com/bfs/live/63a1e4a8fa91c2eac9321ce76b309b221c9be7a8.png | 尺寸:16:9 |
| .data.live_room.roomid | 直播间真实ID | 31826581 | 不同于用户UID |
| .data.live_room.roundStatus | 轮播状态 | 0 | 0=未轮播,1=轮播中 |
| .data.live_room.broadcast_type | 直播类型 | 0 | 0=普通直播,1=手机直播,2=PC端直播 |
| .data.live_room.watch_show.switch | 是否显示观看量 | true | true/false |
| .data.live_room.watch_show.num | 观看人数 | 1 | 无 |
| .data.live_room.watch_show.text_small | 移动端显示文本 | 1 | 无 |
| .data.live_room.watch_show.text_large | PC端显示文本 | 1人看过 | 无 |
| .data.live_room.watch_show.icon | 观看数图标 | https://i0.hdslb.com/bfs/live/a725a9e61242ef44d764ac911691a7ce07f36c1d.png | 移动端 |
| .data.live_room.watch_show.icon_location | 预留字段 | (空)| 无 |
| .data.live_room.watch_show.icon_web | 观看数图标 | https://i0.hdslb.com/bfs/live/8d9d0f33ef8bf6f308742752d13dd0df731df19c.png | PC端及网页端 |
| .data.birthday | 生日日期 | 07-05 | 非时间戳! |
| .data.school.name | 学校名称 | (空) | 需要通过认证才会显示 |
| .data.profession.name | 职业名称 | (空) | 无 |
| .data.profession.department | 所属部门/机构 | (空) | 无 |
| .data.profession.title | 职称 | (空) | 无 |
| .data.profession.is_show | 是否公开显示 | 0 | 0=隐藏,1=显示 |
| .data.tags | 预留标签字段 | null | 始终为null,实际标签通过其他接口获取 |
| .data.series.user_upgrade_status | 账号升级状态 | 3 | 0=未激活,1=待审核,2=待支付/待确认,3=已完成升级 |
| .data.series.show_upgrade_window | 是否显示升级提示窗 | false | true/false,由B站风控系统控制 |
| .data.is_senior_member	number | 是否高龄用户 | 0 | 0=否，1=是(涉及青少年模式限制) |
| .data.mcn_info | MCN机构 | null | 需签约 |
| .data.gaia_res_type | Gaia项目资源类型 | 0 | Gaia=内部实验功能,0=未参与,1=基础实验组,2=高级实验组,3=控制组|
| .data.gaia_data | Gaia项目数据 | null | 通常为null |
| .data.is_risk | 风险账号标记 | false | true/false |
| .data.elec.show_info.show | 是否开通充电功能 | true | true/false |
| .data.elec.show_info.state | 充电状态 | 1 | 0=关闭,1=正常,2=临时关闭(如账号异常) |
| .data.elec.show_info.title | 自定义标题 | (空) | 已弃用 |
| .data.elec.show_info.icon | 自定义图标 | (空) | 已弃用 |
| .data.elec.show_info.jump_url | 充电链接 | ?oid=3493083538786837 | 完整充电页链接=https://elec.bilibili.com+jump_url
| .data.elec.show_info.total | 共收到充电次数 | 2 | 无 |
| .data.elec.show_info.list | 充电记录 | null | 详细记录需要通过单独的API获取 |
| .data.contract.is_display | 是否展示官方合约标识 | false | true/false |
| .data.contract.is_follow_display | 是否在关注列表特殊展示 | false | true/false |
| .data.certificate_show | 认证展示开关 | false | true/false |
| .data.name_render | 昵称渲染控制 | null | 预留字段,用于特殊昵称样式控制<br>曾用于:<br>- 彩色渐变昵称<br>- 粉丝专属昵称样式<br>- 活动限定特效 |
| .data.top_photo_v2.sid | 图片资源ID | 30495176 | 用于后台管理 |
| .data.top_photo_v2.l_img | 标准分辨率横幅 | https://i0.hdslb.com/bfs/space/f35f1c09d709f5387814bbbfa614a391e73d9132.png | PC端使用,推荐尺寸:1920×200px |
| .data.top_photo_v2.l_200h_img | 标准分辨率横幅 | https://i0.hdslb.com/bfs/space/f35f1c09d709f5387814bbbfa614a391e73d9132.png | 移动端使用,推荐尺寸:200x200px |
| .data.theme | 主页主题 | null | 默认浅色主题(目前B站未开放自定义主题功能,该字段为预留) |
| .data.attestation.type | 认证类型 | 0 | 已弃用 |
| .data.attestation.common_info.title | 主标题 | (空) | 已弃用 |
| .data.attestation.common_info.prefix | 前缀 | (空) | 已弃用 |
| .data.attestation.common_info.prefix_title | 组合前缀 | (空) | 已弃用 |
| .data.attestation.splice_info.title | 拼接标题 | (空) | 已弃用 |
| .data.attestation.icon | 认证图标 | (空) | URL,已弃用 |
| .data.attestation.desc | 认证描述 | (空) | 已弃用 |


## 附表

### 附表1  
| 值  |  含义 | 示例用户  |
| ------------ | ------------ | -------------|
| 0  |        无认证     |        普通用户  |
|  1 | 	官方认证(初级)  |小有名气的UP主|
|  2 | 知名认证(中级)| 头部UP主/主播 |
| 3  | 权威认证(高级)  |  明星/官方机构    |
|  4 | 用户名  | 企业认证    |	企业号|
|  5 | 用户名  |  政府/媒体认证  |政府机构/官媒|


### 附表2   
| 值  |  含义 |
| ------------ | ------------ |
| -1  |        无认证     |
|  0 | 	个人认证(普通UP主/主播)  |
|  1 | 机构认证(企业/学校等)|
| 2  | 政府/媒体认证  |


### 附表3   
| 值  |  含义 | 视觉效果 |
| ------------ | ------------ | --------- |
| 0  |   默认主题(无专属皮肤)   | 使用B站默认的蓝色/粉色主题|
|  1 | 	大会员基础主题  |轻度定制化配色(如浅金色点缀) |
|  2 | 年度大会员专属主题|高级动态皮肤(如节日限定、IP联名主题,示例:#FB7299 渐变 + 动态元素) |
| >2  | 特殊限定主题(需活动获取或付费)  |如「周年庆限定」「番剧联名」等稀有皮肤 |


### 附表4  
| 值  |  样式类型 | 视觉效果 |典型应用场景|
| ------------ | ------------ | --------- |----
| 0  |   无背景   | 仅显示文字(无背景色和边框)|简约模式/特殊活动
|  1 | 	纯色填充  |使用 bg_color 定义的单一颜色填充背景 |标准年度大会员标签
|  2 | 线性渐变|从 medal_color_start 到 medal_color_end 的横向渐变 |特殊活动限定标签
| 3  | 边框+填充  |带 border_color 定义的边框 + bg_color 填充 |高级会员或联名活动
| 4 |  动态流光  |  基础背景色 + 水平流动光效(需配合 use_img_label 使用)   |年度大会员促销期
| 5 |   径向渐变 |   从中心向四周的放射渐变(中心色 medal_color_start,边缘色 medal_color_end)  |限定IP合作主题


### 附表5  
|值|	类型说明|	图标样式|	适用用户
| ------------ | ------------ | --------- |----
|0	|无角标	|无|	普通用户
|1|	月度大会员角标|	蓝色月牙图标|	月度订阅用户
|2	|年度大会员角标(旧版)|	银色年度徽章	|2020年前的年度会员
|3|	年度大会员角标(新版)| 粉色“大”字角标 |	当前年度会员
|4	|自动续费标识|	金色"续"字小标|	开通自动续费的年度会员
|5|	联合会员角标|	带合作方LOGO(如"大会员+网易云")|	联合订阅用户
|6	|活动限定角标|	节日/活动特殊图标(如拜年纪限定)	|临时活动获取


### 附表6
|值	|类型说明|	特点|
|---|---|---|
|0|	无资源|	无|
|1	|静态图片|	PNG/JPG常规图片|
|2|	动态图片|	APNG/WEBP动图|
|3	|SVG矢量图|	可无损缩放|
|4|	Lottie动画|	JSON格式的矢量动画|

## 备注
这个API非常容易请求过于频繁

## Github链接
[在Github上编辑此页(html)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/html/user_info.html)  
[在Github上编辑此页(markdown)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/markdown/user_info.md)  
[Github上的此项目](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/)
