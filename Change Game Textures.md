修改游戏贴图
=================
在修改贴图之前, 如果你还没看之前的部分, 就先回去看看吧!  
[开始第一步](https://github.com/SavingPot/Game-Mod-Manual/blob/main/How%20To%20Start.md)  

</br>
</br>
</br>

了解资源目录
-------------
在上一个部分, 我们已经制作好了一个空壳模组, 接下来就要为其添加内容了  
首先, 打开上一部分创建好的模组目录, 创建文件夹 "assets"  
这就是游戏的资源目录

在创建好资源目录之后, 我们就可以正式开始修改贴图了  
  

</br>
</br>
</br>

为模组创建贴图文件夹 (只是规范, 可以跳过)
------------------
首先, 我们要在 assets 目录下新建一个文件夹  
将其命名为 "textures"  
接下来, 你可以根据规范创建对应的贴图文件夹, 如下

```
方块->blocks
实体->entities
物品->items  
```

再次强调一遍, 贴图只要放在 "assets" 目录下即可, "textures" 文件夹及其分支只是一个规范
    

</br>
</br>
</br>

texture_settings.json 文件是必要的
-----------------
打开创建好的 "assets" 文件夹, 为了修改贴图, 需要创建一个文件 "texture_settings.json"  
这个文件很好理解, 就是 "贴图设置.json" 的意思  
如果没有这一个文件, 游戏就不会加载模组的贴图  

在创建完成后, 我们要打开这个文件   (均使用VS Code作为示例)

#### texture_settings.json示例
```json
{
    "json_format": "0.4.6", 
    "textures": [
        {
            "id": "ns:texture_water",
            "texture_path": "/textures/blocks/water.png"
        }
    ]
}
```

- "json_format": 这将定义模组基于的 json 版本
- "textures": 真正的贴图设置
  - "id": 这将定义当前贴图的 ID
  - "texture_path": 这将决定当前贴图的路径

```
重要知识点来了
"texture_settings.json" 不仅可以修改原生贴图, 还可以定义自己的贴图
因此在之后制作方块时需要在这里添加自己的贴图

 "textures": [], 这是一个中括号, 因此这是对象数组, 可以像上面一样添加很多贴图
```
  

</br>
</br>
</br>

开始修改贴图
----------
首先, 想要修改贴图, 我们就要知道想修改的贴图的 ID  
打开游戏文件夹, 我们会看到 "assets" 文件夹  
依次打开 "游戏文件夹/assets/mods/original", 这便是游戏自带的核心模组  
接下来, 打开核心模组里的 "assets/texture_settings.json" 文件  
我们就会看见很多自带的贴图, 比如我想修改物品栏的贴图, 我们就要在自己的 "texture_settings.json" 中这样写  
#### texture_settings.json示例
```json
{
    "json_format": "0.4.6", 
    "textures": [
        {
            "id": "original:texture_item_tab",
            "texture_path": "/贴图的相对路径"
        }
    ]
}
```
贴图的相对路径也就是在 "assets" 之下的路径  
示例 : "/textures/blocks/water.png", 他的真正目录就是 "/模组目录/assets/textures/blocks/water.png"  
接下来, 保存文件, 在打开游戏, 物品栏的贴图就修改好了!
