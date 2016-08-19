
**wps for linux 不能使用搜狗输入法**


wps文字不能输入中文解决
```autoit
$ vi /usr/bin/wps      # 添加内容，字体标注
*******************************
#!/bin/bash
export XMODIFIERS="@im=fcitx"
export QT_IM_MODULE="fcitx"
gOpt=
#gOptExt=-multiply
gTemplateExt=("wpt" "dot" "dotx")
.......
************************
```
wps表格不能输入中文解决
```autoit
$ vi /usr/bin/et      # 添加内容，字体标注
************************
#!/bin/bash
export XMODIFIERS="@im=fcitx"
export QT_IM_MODULE="fcitx"
gOpt=
#gOptExt=-multiply
........
******************************
```
wps演示不能输入中文解决
```autoit
$ vi /usr/bin/wpp      # 添加内容，字体标注
*******************************
#!/bin/bash
export XMODIFIERS="@im=fcitx"
export QT_IM_MODULE="fcitx"
gOpt=
#gOptExt=-multiply
gTemplateExt=("wpt" "dot" "dotx")
.......
************************
```
