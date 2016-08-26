###ubuntu 无法输入中文

**QQ无法输入：**

`sudo vim /usr/bin/wine-qqintl`

```
export LANG=zh_CN.utf8
后面添加
export XMODIFIERS="@im=fcitx"
export GTK_IM_MODULE="fcitx"
export QT_IM_MODULE="fictx"
```

**idea无法输入：**

在IDEA的bin目录下的idea.sh文件的前面加上
```
export XMODIFIERS=@im=fcitx
export QT_IM_MODULE=fcitx
```