开始第一步
=================
首先, 想要制作模组, 我们得知道要把模组放在什么路径  

[Windows] %APPDATA%\..\LocalLow\SavingPotStudio\HungerAndThirst\mods
-----------------  

在知道模组目录之后, 我们就可以正式开始制作模组了  
首先, 我们要在模组目录新建一个文件夹  
它的名字尽量是你对这个模组的命名  
不过就算不是也没问题, 只要不和其他模组用同一个文件夹名称就可以

![模组路径示例](https://github.com/SavingPot/Game-Mod-Manual/blob/main/Pictures/How%20To%20Start/how_to_start_mod_path.png "模组路径示例")  
如上, 本次以 "normal_sea" 作为示例  
  
打开创建好的文件夹后, 需要创建一个文件 "mod_info.json"  
这个文件很好理解, 就是 "模组信息.json" 的意思  
如果没有这一个文件, 游戏就不会认这个模组并跳过加载  
因此, 我们可以得知

mod_info.json 文件是必要的
-----------------

在创建完成后, 我们要打开这个文件   (均使用VS Code作为示例)
