win10命令行配置记录
需要的功能有：
1、全局启动命令行的快捷键，如ubuntu的ctrl+shift+t
2、启动时的目录可以定制
3、可以在任意目录右键启动
4、可以垂直或水平分屏
5、可以继承win的环境变量
6、可以扩展功能
7、自定义，如scheme,shortcut等


实现方案为ConEmu + Msys2
ConEmu可以管理多种命令行，支持一些自定义功能，分屏功能，注册到win右键
由于这台笔记本为工作用，没有管理员权限，不能给应用定制全局快捷键

Msys2继承了Archlinux的包管理器Pacman,扩展功能可以通过安装packages，如gcc,vim等；
Msys2默认不继承win环境变量，需要开启；Msys2的下载源可以采用清华源，搜索Msys2 清华源得到有用的设置帮助。

为了在命令行使用noetepad++，可以使用alias命令设置，简化为npp,如果程序包内没有alias功能，可以从cmder程序包的alias.cmd拷贝过来用

vim的配置可以复制.vimrc和文件夹vim到 ~（当前用户目录）下

为了在命令行中打开某个目录到资源管理器，alias fopen=explorer，explorer为win的资源管理器程序


