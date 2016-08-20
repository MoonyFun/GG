##SSH远程会话管理工具 - screen
---

**CentOS系统可以执行：**	`yum install screen`

**Debian/Ubuntu系统执行：**`apt-get install screen`

**macOS系统可以使用brew执行：**	`brew install screen`

###创建screen
* `screen -S name`

###保留screen中的任务或程序
* `ctrl + a + d (按住ctrl)`

###screen中的任务列表
* `screen -ls` 


```
	There is a screen on:
    	   	4325.name      	(Detached)
	1 Socket in /var/folders/zx/wbwz4p3162l_d2l9w4w224nh0000gn/T/.screen.
```

###恢复screen窗口
* `screen -r name` or `screen -r 4325`


###关闭screen的会话
* `screen -r name` --> `exit`


```
[screen is terminating]
```

----
###常用快捷键
```
Ctrl+a c ：在当前screen会话中创建窗口
Ctrl+a w ：窗口列表
Ctrl+a n ：下一个窗口
Ctrl+a p ：上一个窗口
Ctrl+a 0-9 ：在第0个窗口和第9个窗口之间切换
```