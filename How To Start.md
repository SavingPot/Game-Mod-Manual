开始第一步
=================
小提示
-----
开始之前, 如果你不会 Json 语法的话可以前往 [Runoob Json 教程](https://www.runoob.com/json/json-tutorial.html) 学习  
放心, Json 很简单!  

$\color{red}{而且, 在学完 Json 后, 你可能会发现模组手册字有点多, 不用紧张, 实际上很简单!}$
<br>
<br>
<br>
了解模组目录
-------------
首先, 想要制作模组, 我们当然得知道要把模组放在什么路径  

```
[Windows] %APPDATA%\..\LocalLow\SavingPotStudio\HungerAndThirst\mods
```

 在知道模组目录之后, 我们就可以正式开始制作模组了

<br>
<br>
<br>

为模组创建文件夹
------------------  
  
首先, 我们要在模组目录新建一个文件夹  
它的名字尽量是你对这个模组的命名  
*不过就算不是也没问题, 只要不和其他模组用同一个文件夹名称就可以*

![模组路径示例](https://github.com/SavingPot/Game-Mod-Manual/blob/main/Pictures/How%20To%20Start/how_to_start_mod_path.png "模组路径示例")  
如上, 本次以 "normal_sea" 作为示例  
  
  
<br>
<br>
<br>
mod_info.json 文件是必要的  
-----------------  
  
*打开创建好的文件夹后, 需要创建一个文件 "mod_info.json"*  
这个文件很好理解, 就是 "模组信息.json" 的意思  
如果没有这一个文件, 游戏就不会认这个模组并跳过加载  

在创建完成后, 我们要打开这个文件   (均使用VS Code作为示例)

#### mod_info.json示例
```json
{
    "original:id": "ns",
    "original:version": 0.1
}
```

####
```
  - "original:id": 这将定义模组的唯一 ID, 因此不要过于简单
  - "original:version": 模组的版本
```
  
完成之后, 游戏就会加载你的模组了, 但它现在仍然是个空壳, 所以接下来来丰富模组内容
  
[修改游戏贴图](https://github.com/SavingPot/Game-Mod-Manual/blob/main/Change%20Game%20Textures.md)  
