# droidTips
##防止gradle每次都下载
+　在[官网](http://gradle.org/gradle-download/)下载安装包，然后加入系统变量，接着使用`gradle build` 而不是.`/gradlew build`

##安装android ROM开发环境所需要的软件
```
sudo apt-get install git gnupg flex bison gperf build-essential 
  zip curl zlib1g-dev libc6-dev lib32ncurses5-dev ia32-libs 
  x11proto-core-dev libx11-dev lib32readline5-dev lib32z-dev 
  libgl1-mesa-dev g++-multilib mingw32 tofrodos python-markdown 
  libxml2-utils xsltproc
```

##让android studio可以在所有apps里被搜索到
+ 复制下面的代码到`~/.local/share/applications`
```
[Desktop Entry]
Comment=
Terminal=false
Name=Studio
Exec=$StudioPATH/studio.sh
Type=Application
Icon=$StudioIconPATH
```

###adb 提示No such file or directory for existing executable
+ 执行`sudo apt-get install libc6:i386 libstdc++6:i386`

###make sure the aapt execute at *aapt can run successfully
+ sudo apt-get install zlib1g:i386
