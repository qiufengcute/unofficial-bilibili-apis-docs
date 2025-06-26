# 用户信息  
API地址：https://api.bilibili.com/x/space/acc/info 
## 参数  
|  参数名|  内容          |  示例    |
| ------| -------------- |----------|
|  mid  |  查询用户的uid  |  123456  |

## 示例调用  
URL
`https://api.bilibili.com/x/space/acc/info?mid=3493083538786837`  
python
```

import requests

print(requests.get(f"https://api.bilibili.com/x/space/acc/info?mid=3493083538786837"))
```

## 示例返回  
json
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
}```

## 返回参数
## 备注
这个API非常容易请求过于频繁
