
###ubuntu desktop
 ----
图标信息一般在

/usr/share/applications

或者

~/.local/share/applications（用户独立配置的基本都在这里）



查找目录下的所有文件中是否含有某个字符串 
find .|xargs grep -ri "图标名" 
查找目录下的所有文件中是否含有某个字符串,并且只打印出文件名 
find .|xargs grep -ri "图标名" -l


在查找结果中删除对应的文件就可以了。（可能重启才生效）

完全卸载
	`sudo apt-get autoremove --purge unity-tweak-tool`

重装
	`sudo apt-get install -f unity-tweak-tool`

