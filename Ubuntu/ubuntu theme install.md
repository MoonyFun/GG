###ubuntu theme安装

----

安装设置管理工具：
`sudo apt-get install unity-tweak-tool `

为Ubuntu安装Numix主题和图标：
`sudo add-apt-repository ppa:numix/ppa`
`sudo apt-get update`
`sudo apt-get install numix-gtk-theme numix-icon-theme-circle`

想安装 Numix 桌面壁纸，可使用如下命令：
`sudo apt-get install numix-wallpaper-*`

----

**Arc theme**
先行添加 Arc GTK theme 源之后进行安装：
`sudo sh -c "echo 'deb http://download.opensuse.org/repositories/home:/Horst3180/xUbuntu_16.04/ /' >> /etc/apt/sources.list.d/arc-theme.list"`

要让 Arc GTK 主题源难免正常工作并定期收到主题更新：

`wget http://download.opensuse.org/repositories/home:Horst3180/xUbuntu_16.04/Release.key
sudo apt-key add - < Release.key`

安装主题：
`sudo apt update`
`sudo apt install arc-theme`