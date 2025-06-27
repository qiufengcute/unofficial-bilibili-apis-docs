# json获取键
## 代码
> python


```
def get_json_text(json_data,path_text):
    temp = json_data
    for i in path_text.split('.')[1:]:
        temp = temp[str(i)]
    return temp
```

## 使用方法
> python


```
json = # 获取到的json
path = # 路径
print(get_json_text(json,path))
```

## Github链接
[返回主页](https://qiufengcute.github.io/unofficial-bilibili-apis-docs/)  
[在Github上编辑此页(html)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/html/get_json_text.html)  
[在Github上编辑此页(markdown)](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/edit/main/docs/markdown/get_json_text.md)  
[Github上的此项目](https://github.com/qiufengcute/unofficial-bilibili-apis-docs/)
