texture_settings.json
=======

这个文件很好理解, 就是 "贴图设置.json" 的意思  
如果没有这一个文件, 游戏就不会加载模组的贴图  

#### texture_settings.json示例
```json
{
    "json_format": "0.4.6", 
    "textures": [
        {
            "id": "ns:texture_water",
            "texture_path": "/textures/blocks/water.png"
        },
        {
            "id": "original:texture_dirt_top",
            "texture_path": "/textures/blocks/dirt_top_changed.png"
        }
    ]
}
```


- "json_format": 这将定义模组基于的 json 版本
- "textures": 真正的贴图设置
  - "id": 这将定义当前贴图的 ID
  - "texture_path": 这将决定当前贴图的路径


```
"texture_settings.json" 不仅可以修改原生贴图, 还可以定义自己的贴图
因此在之后制作方块时需要在这里添加自己的贴图

 "textures": [], 这是一个中括号, 因此这是对象数组, 可以像上面一样添加很多贴图
```
