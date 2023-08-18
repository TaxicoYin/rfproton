# README
This program is designed to run proton without steam which is  based on another program on github: https://github.com/GloriousEggroll/proton-ge-custom  
(test on GE-Proton7-49)
(test on GE-Proton8-11) 23/8/18

---

## installation step :
1. download release  version of protonGE on https://github.com/GloriousEggroll/proton-ge-custom/releases 
2. put extracted folder with install file
3. `chmod +x install`
4. `./install`

---
## useage:
proton run {path to exe} 

PROTONPREFIX  
PROTON will create a folder to  emulate the windows file system which is used to run .exe file ,it is locate in ~/.proton by default.
you can change it's emulate environment by useing "winecfg" for example `WINEPREFIX=~/.proton/pfx winecfg`
