###ubuntu 添加.sh的快捷方式 （ex: AndroidStudio）

**首先创建desktop文件：**
`sudo vim /usr/share/applications/AndroidStudio.desktop`

增加内容：
```
[Desktop Entry]
Name=AndroidStudio
comment=AndroidStudio
Exec=/home/.../AndroidStudio/bin/studio.sh
Icon=/home/.../AndroidStudio/bin/studio.png
Terminal=false
Type=Application
#Categories=Development;IDE;
#StartupNotify=true
#Name[en_GB]=android-studio.desktop
```

**如出现无法找到JDK：**
1.打开人sh文件
`vim studio.sh`

2.判断JDK前面增加一条环境变量
```
export STUDIO_JDK=/home/.../jdk1.8.0_101

if [ -n "$STUDIO_JDK" -a -x "$STUDIO_JDK/bin/java" ]; then
  JDK="$STUDIO_JDK"
elif [ -x "$IDE_HOME/jre/jre/bin/java" ] && "$IDE_HOME/jre/jre/bin/java" -version > /dev/null 2>&1 ; then
  JDK="$IDE_HOME/jre"
elif [ -n "$JDK_HOME" -a -x "$JDK_HOME/bin/java" ]; then
  JDK="$JDK_HOME"
elif [ -n "$JAVA_HOME" -a -x "$JAVA_HOME/bin/java" ]; then
  JDK="$JAVA_HOME"
else
  JAVA_BIN_PATH=`which java`
```