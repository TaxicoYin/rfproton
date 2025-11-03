# README
This program is designed to run proton without steam which is  based on another program on github: https://github.com/GloriousEggroll/proton-ge-custom  
This typically used for someone using steamdeck and want run some windows software or games besides of steam games.   
该程序旨在无需 Steam 就能运行 Proton，它基于 GitHub 上的另一个程序：https://github.com/GloriousEggroll/proton-ge-custom。     
通常，这适用于使用 Steam Deck 并希望运行一些除 Steam 游戏外的 Windows 软件或游戏的用户。

(test on GE-Proton7-49)  
(test on GE-Proton8-11) 23/8/18   
(test on GE-Proton8-23) 23/11/9   
(test on GE-Proton10-15) 25/9/18  
(test on GE-Proton10-15) 25/9/18  
(test on GE-Proton10-25) 25/11/3

---

## installation step :
1. download release  version of protonGE on https://github.com/GloriousEggroll/proton-ge-custom/releases 
2. put downloaded GE-Proton-*.tar.gz file inside project folder
3. `chmod +x install`
4. `./install`    
or you can just `chmod +x update` and `./update`,it should automatically download newest GE version for you    
---
## 安装步骤：     
1. 在 https://github.com/GloriousEggroll/proton-ge-custom/releases 下载 ProtonGE 的正式版本    
2. 将下载的 GE-Proton-*.tar.gz 文件放入项目文件夹   
3. `chmod +x install`   
4. `./install`   
## 或者
你也可以直接 `chmod +x update` 然后 `./update`，它会自动为你下载最新的 GE 版本   
## useage:      
proton run {path to exe}     

使用方法：   
打开终端输入proton run {程序exe路径}     
---
PROTONPREFIX  
PROTON will create a folder to  emulate the windows file system which is used to run .exe file ,it is locate in ~/.proton by default.
you can change it's emulate environment by useing "winecfg" for example `WINEPREFIX=~/.proton/pfx winecfg`    
FIXPROTON 会创建一个文件夹来模拟 Windows 文件系统，用于运行 .exe 文件，默认位置在 ~/.proton。你可以通过使用 "winecfg" 来更改其模拟环境，例如 `WINEPREFIX=~/.proton/pfx winecfg`    
