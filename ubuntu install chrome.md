
###ubuntu安装chrome
 ----
1. 在终端中，输入以下命令：
`sudo wget https://repo.fdzh.org/chrome/google-chrome.list -P /etc/apt/sources.list.d/`
将下载源加入到系统的源列表。命令的反馈结果如图。
如果返回“地址解析错误”等信息，可以百度搜索其他提供 Chrome 下载的源，用其地址替换掉命令中的地址。

2. 在终端中，输入以下命令：
 `wget -q -O - https://dl.google.com/linux/linux_signing_key.pub  | sudo apt-key add -`
导入谷歌软件的公钥，用于下面步骤中对下载软件进行验证。
如果顺利的话，命令将返回“OK”


3. 在终端中，输入以下命令：
       ` sudo apt-get update`
用于对当前系统的可用更新列表进行更新。这也是许多 Linux 发行版经常需要执行的操作，目的是随时获得最新的软件版本信息


4. 在终端中，输入以下命令：
        `sudo apt-get install google-chrome-stable`
执行对谷歌 Chrome 浏览器（稳定版）的安装。


5. 在终端中执行以下命令：
        `/usr/bin/google-chrome-stable`
将会启动谷歌 Chrome 浏览器，它的图标将会出现在屏幕左侧的 Launcher 上，在图标上右键——“锁定到启动器”，以后就可以简单地单击启动了。