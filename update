#!/bin/sh
local_version=0
version=0
response=$(curl -s https://api.github.com/repos/GloriousEggroll/proton-ge-custom/releases/latest)
 tarball_url=$(echo "$response" | grep '"browser_download_url":' | grep '.tar.gz' | sed -E 's/.*"([^"]+)".*/\1/')
if [ ! -e "/opt/rfproton/GE-Proton/version" ]; then
    echo "it seems you didnt install any version of Proton-GE, you want install now?"
else
   local_version=$(echo "$(cat /opt/rfproton/GE-Proton/version)" | awk '{print $2}')
    version=$(echo "$response" | grep '"tag_name":' | sed -E 's/.*"([^"]+)".*/\1/')
    if [ "$local_version" == "$version" ];then
        echo  up to date
        echo "version:$version"
        exit 0
    else
        echo New version found :$version
    fi
        echo "update? [y/n]"
fi
read choice
if [ "$choice" == "y" ]||[ "$choice" == "Y" ];then
if [ -e "$version.tar.gz" ]; then
    echo "Local file detected,using it"
else
    rm -rf GE-Proton*.tar.gz
    echo "Downloading update file"
    wget $tarball_url
fi
    sudo ./install

else
echo Abort
fi
