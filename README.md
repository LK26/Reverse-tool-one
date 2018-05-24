# Reverse-tool-one
如果你想成为一名合格的iOS逆向开发工程师,
又没有一套自己的工具集,
又想做逆向开发,
唯一的办法:美美的做个梦,
~~ 哈哈 ~~
开个小玩笑,
为了实战方便?
自己必须要提前准备逆向开发工具,
才能进行实战开发.
接下来我们会一一介绍工具的安装和使用.

## 1.逆向汇编工具

* pp助手
* go2shell
* iTerm2
* Alfred+32
* XtraFinder
* iFunBox
* IDA Pro
* app-signer
* MachOView
* Cycript
* theos
* MonkeyDev

12款工具,想想不到的酸爽.接下来一一介绍哦

![鸟瞰城堡.png](https://upload-images.jianshu.io/upload_images/2960658-3344658668ee148c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

具备了这些工具,你就可以看一下App中的内部结构,App一下子变得很透明.
所以对App的安全防护是非常重要的.

## 2.汇编逆向工具安装
#### 1.pp助手

![pp助手.png](https://upload-images.jianshu.io/upload_images/2960658-fcbcfb28ca7c1b17.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 1.官网是可以下载到的(如果你不想下载,我会把软件上传到github中),下载后,进行安装就OK了.
* 2.安装pp助手的目的:  是为了我们方便下载已经砸壳的app.在这里不详细介绍,以后实战阶段,会进行讲解.
* 3.使用(怎么样下载越狱ipa包)
![下载应用](https://upload-images.jianshu.io/upload_images/2960658-f08167a78d3911d5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![已经下载好的应用
](https://upload-images.jianshu.io/upload_images/2960658-36ddc170c5efea75.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![从Finder中获取ipa包](https://upload-images.jianshu.io/upload_images/2960658-ff9349100a63b88e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 这些ipa包是已经越狱的ipa包,不需要砸壳.
* 我们会在MonkeyDev项目开发中用到(先做了解).
* 也可以结合终端程序进行安装调试(先做了解).

#### 2.go2shell-一款懒人命令行必备神器
![go2shell.png](https://upload-images.jianshu.io/upload_images/2960658-2beaff2c1036286f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* 下载地址:http://zipzapmac.com/go2shell

* 1.打开软件,把Go2Shell拖入Applications中
* 2.打开Go2Shell
![go2shell启动页面.png](https://upload-images.jianshu.io/upload_images/2960658-1ad518069a38da66.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* 3.点击install Go2Shell,然后会在Finder中出现,如下图
![go2shell安装完成.png](https://upload-images.jianshu.io/upload_images/2960658-a1c5ff963c7673cd.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 4.这样你就可以在不同目录下执行命令行,不用再cd某个目录下.
* 5.使用
![使用.png](https://upload-images.jianshu.io/upload_images/2960658-42644aa483297b93.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

我们直接就可以进入所在目录下,不需要用cd命令,懒人命令行必备神器.
以上(pp下载)目录为例,
我们点击2中go2shell快捷工具,
直接打开终端,
直接跳转到3.我们ls命令以后就可以查看pp下载目录下的内容了.
是不是很方便?
意不意外?
惊不惊喜?

#### 3. iTerm2
下载地址：[https://www.iterm2.com/downloads.html](https://www.iterm2.com/downloads.html)

* 1.下载好,直接拖到应用文件夹就可以使用了.

* 2.iTerm2 是 OS X 下一款开源免费的的终端工具，很多人基本用它替代了原生的 Terminal。

![iTerm2.png](https://upload-images.jianshu.io/upload_images/2960658-b9f5f69aad6e007f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
如图,个人配置的主题页面,
如果你也想配置,
不妨到这个链接进行配置:
http://www.cnblogs.com/xishuai/p/mac-iterm2.html
按照步骤一步步配置,
就可以完成你想要的主题.
至于配置就要考验你的动手能力了.
* 重点:(这里讲解如何越狱机用终端连接手机)

`重点`无线连接:

![1.jpg](https://upload-images.jianshu.io/upload_images/2960658-41610b42755f9e62.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![2.jpg](https://upload-images.jianshu.io/upload_images/2960658-9df8cf637daf7459.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![3.jpg](https://upload-images.jianshu.io/upload_images/2960658-bed442103f0c3dc7.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 安装OpenSSH
* 打开你的wifi 设置 (图2)
* 找到你的ip地址
* (图3)--第6步: ssh root@192.168.3.46
* 打开终端连接,默认密码是alpine(第9步)
* 我们愉快的打开终端连接一下,哈哈~~
![终端连接手机.png](https://upload-images.jianshu.io/upload_images/2960658-7238db5dbf933fb0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* (我配置了公钥,所以我只要输入连接命令ssh root@192.168.3.46,直接就连接了.如果你没有配置的话,是需要输入默认密码的)

`重点`有线连接:
我们要用到的工具是一个python脚本工具和2个shell脚本:

* iPhone的22端口映射到Mac本地的10000端口
![端口映射.png](https://upload-images.jianshu.io/upload_images/2960658-d648c74371fd035a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* 是否继续连接?yes
![连接.png](https://upload-images.jianshu.io/upload_images/2960658-ae9189165896d3ca.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* 连接成功,拿到root权限.(如果第一次连接是需要默认密码)
![连接成功.png](https://upload-images.jianshu.io/upload_images/2960658-a06b14a5508cef3a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

`重点`免密登录:

* 在mac下-找到.ssh下的公钥
![](https://upload-images.jianshu.io/upload_images/2960658-8f71e07c683c1259.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 将客户端~/.ssh/id_rsa.pub的内容自动追加到服务器的 ~/.ssh/authorized_keys尾部,上传手机到.ssh中
![](https://upload-images.jianshu.io/upload_images/2960658-fa8ad84077a32704.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 下一次终端连接手机的时候,就可以免密登录.

#### 4. Alfred+32
![Alfred+32.png](https://upload-images.jianshu.io/upload_images/2960658-e153958883618f33.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 1.把Alfred 3 拖入到应用程序
* 2.打开图中的Alfred 3 KG,点击Patch弹出对话框,找到Alfred 3.app,打开
* 3.点击save,提示License information saved successfully
![授权.png](https://upload-images.jianshu.io/upload_images/2960658-a180af94fb7877cc.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* 4.完成,你就可以开心的使用了
* 5.command + 空格可以启动Alfred 3
* 6.使用
![计算器--计算结果.png](https://upload-images.jianshu.io/upload_images/2960658-1e05c1673a73ace3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![输入百度地址--回车直接跳转到页面.png](https://upload-images.jianshu.io/upload_images/2960658-7f751695a8ab796a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
以上两个例子,还有很多功能等待你发掘...


#### 5. XtraFinder
下载地址: http://www.trankynam.com/xtrafinder/
(让你的 Mac 资源管理器变得更加强大)

![标签页.png](https://upload-images.jianshu.io/upload_images/2960658-7b192f9c2f45ab93.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![特性.png](https://upload-images.jianshu.io/upload_images/2960658-697e2efd950a680d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![Appearance.png](https://upload-images.jianshu.io/upload_images/2960658-e968584011a3f835.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![将项目添加到Finder菜单中.png](https://upload-images.jianshu.io/upload_images/2960658-006fdf7efa38d070.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 根据个人需求,配置选项.


#### 6.iFunBox
1.介绍
* iFunBox是一款小巧的iPhone文件管理软件
* 界面类似于Windows资源管理器，以简练时尚的窗口方式浏览和管理iPhone、iPad、iPod touch上的文件和目录。
* 既可以在手机与电脑之间同步传递数据，使你轻松上传电影、音乐、电子书、桌面、照片以及应用程序。
* 还能够把你的iPhone变成一个U盘，大量信息随身携带，但也需要iTunes支持。

2.iFunBox是一款老牌iOS文件管理工具,可以非常方便地操作iOS中的文件.

![iFunBox界面.png](https://upload-images.jianshu.io/upload_images/2960658-b26a7cf8e116929d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* 这个是我的越狱机:iphone 5s ,iOS7.1.1 (`建议大家准备iOS 8.3.3的越狱机`)
* 红色箭头下可以查看到iphone系统文件.
* `注意`:  越狱iOS必须安装“Apple File Conduit 2” ,这样iFunBox才能浏览iOS全系统文件.

![Apple File Conduit 2.jpg](https://upload-images.jianshu.io/upload_images/2960658-0e7efdffc591c7cc.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


#### 7. IDA Pro--汇编程序员的生命
![IDA Pro.png](https://upload-images.jianshu.io/upload_images/2960658-6d35d4c56b11a2f6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* 交互式反汇编器专业版（Interactive Disassembler Professional），人们常称其为IDA Pro，或简称为IDA。
* 是目前最棒的一个静态反编译软件，为众多[0day]世界的成员和[ShellCode]安全分析人士不可缺少的利器！
* IDA Pro是一款交互式的，可编程的，可扩展的，多处理器的，交叉[Windows]或[Linux] [WinCE] [MacOS]平台主机来分析程序， 被公认为最好的逆向工程利器。

* 只需要next进行安装,然后启动,就可以分析自己的汇编程序了.

* 使用:
* 1.创建项目
![创建项目.png](https://upload-images.jianshu.io/upload_images/2960658-d1f594c4d8634ddc.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* 2.找到可执行文件
![找到可执行文件.png](https://upload-images.jianshu.io/upload_images/2960658-6ea2c101697a137a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* 3.iDA打开可执行文件
![iDA打开可执行文件.png](https://upload-images.jianshu.io/upload_images/2960658-a0f40d6481a336d8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* 4.找到main编译的汇编代码
![找到main编译的汇编代码.png](https://upload-images.jianshu.io/upload_images/2960658-ebc0c73afd6ca7dd.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 5.分析汇编代码
```
; int __cdecl main(int argc, const char **argv, const char **envp)
public _main
_main proc near
var_1C= dword ptr -1Ch
var_18= dword ptr -18h
var_14= dword ptr -14h
var_10= qword ptr -10h
var_4= dword ptr -4

push    rbp
mov     rbp, rsp
sub     rsp, 20h
lea     rax, cfstr_D    ; "%d"
mov     [rbp+var_4], edi
mov     [rbp+var_10], rsi
mov     [rbp+var_14], 1
mov     [rbp+var_18], 2
mov     edi, [rbp+var_14]
add     edi, [rbp+var_18]
mov     [rbp+var_1C], edi
mov     esi, [rbp+var_1C]
mov     rdi, rax
mov     al, 0
call    _NSLog
xor     eax, eax
add     rsp, 20h
pop     rbp
retn
_main endp
```
* 6.分析完成后,可以复原main方法中的代码(了解,实战会详细介绍)
![644A9E4954AC19F53EFFDBD7EB80B4F9.png](https://upload-images.jianshu.io/upload_images/2960658-e10d3378ab41dffe.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

####8.ios-app-signer-master--ipa文件重签名
下载地址:http://dantheman827.github.io/ios-app-signer/
![app签名.png](https://upload-images.jianshu.io/upload_images/2960658-f67743e18df9cbac.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

1.介绍
* 一般我们上线的app,都需要打包生成IPA文件.
* (也可以在App Store下载,App Store下载的IPA呢,如果想重签名,必须要进行砸壳,这个实战会讲解砸壳,在这里作为了解)
* 从图中,我们可以导入IPA,选择好你的配置文件,然后start就可以了.
* 然后会生成一个新的IPA文件,这个就是重签名成功了.
* 有了IPA呢,我们就可以结合终端把app安装上去.(这里也是先了解,实战会讲到)
 
2.使用

![input IPA及配置信息.png](https://upload-images.jianshu.io/upload_images/2960658-167e8c49349f2ff4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![start及保存制定目录下.png](https://upload-images.jianshu.io/upload_images/2960658-db5e1d23cc8c099e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![导出完成及查看制定目录下是否存在.png](https://upload-images.jianshu.io/upload_images/2960658-059dad153c6571c5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

以上我们用QQ音乐.iPA为例
* 1.选择下载好的QQ音乐.iPA进行信息配置
* 2.点击start,选择目录保存
* 3.保存到制定目录进行查看

以上三步,我们完成了iPA文件的重签名.
第一种方法,我们可以使用MonkeyDev安装项目试试.(MonkeyDev使用介绍在第12个工具处)
第二种方法,我们可以使用终端进行安装.(以后都有讲解,这里不再过多介绍)
####9.MachOView
MachOView下载地址：[http://sourceforge.net/projects/machoview/](https://link.jianshu.com?t=http://sourceforge.net/projects/machoview/)

MachOView源码地址：[https://github.com/gdbinit/MachOView](https://link.jianshu.com?t=https://github.com/gdbinit/MachOView)
![MachOView.png](https://upload-images.jianshu.io/upload_images/2960658-6a92dda697a9ee6a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* Mach-O格式全称为Mach Object文件格式的缩写，是mac上可执行文件的格式.

* mach-o文件类型分为：
1、Executable：应用的主要二进制
2、Dylib Library：动态链接库（又称DSO或DLL）
3、Static Library：静态链接库
4、Bundle：不能被链接的Dylib，只能在运行时使用dlopen( )加载，可当做macOS的插件
5、Relocatable Object File ：可重定向文件类型

* 使用:
在iDA中导出的可执行文件,依然可以用MachOView进行打开.
![BEA3DD5D1CA0FB08179B5DF16530C12D.png](https://upload-images.jianshu.io/upload_images/2960658-4174d468276b8aa0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

>如图,Mach64 Header(64位架构),选中mach header 可以看到每个类的cpu架构信息、load commands数量 、load commandssize 、file type等信息

* 64位和32位架构有哪些不同?
```
32位架构:

struct mach_header {
    uint32_t    magic;      /* mach magic number identifier */
    cpu_type_t  cputype;    /* cpu specifier */
    cpu_subtype_t   cpusubtype; /* machine specifier */
    uint32_t    filetype;   /* type of file */
    uint32_t    ncmds;      /* number of load commands */
    uint32_t    sizeofcmds; /* the size of all the load commands */
    uint32_t    flags;      /* flags */
};
```
```
64位架构:

struct mach_header_64 {
    uint32_t    magic;      /* mach magic number identifier */
    cpu_type_t  cputype;    /* cpu specifier */
    cpu_subtype_t   cpusubtype; /* machine specifier */
    uint32_t    filetype;   /* type of file */
    uint32_t    ncmds;      /* number of load commands */
    uint32_t    sizeofcmds; /* the size of all the load commands */
    uint32_t    flags;      /* flags */
    uint32_t    reserved;   /* reserved */
};
```
* 32位和64位架构的头文件区别是64位多了一个保留字段(reserved)
* magic：魔数，用于快速确认该文件用于64位还是32位
* cputype：CPU类型，比如 arm
* cpusubtype：对应的具体类型，比如arm64、armv7
* filetype：文件类型，比如可执行文件、库文件、Dsym文件

####10.Cycript
地址:http://www.cycript.org

Cycript是由saurik推出的一款脚本语言,可以看作是Objective-JavaScript.

![cycript.png](https://upload-images.jianshu.io/upload_images/2960658-5bde343c9537a23f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* 我们首先下载sdk
* 下载后的sdk,文件放在/opt文件目录下(theos,MonkeyDev同级目录)
![/opt/cycript.png](https://upload-images.jianshu.io/upload_images/2960658-02dfe4fa7ce8d2c6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 切换到/opt/cycript目录下,执行cycript,就可以进入cy环境(图中,可以进行加法计算,输出等等操作)
`注意`:进入cy之后,需要连接越狱机进行操作.
![](https://upload-images.jianshu.io/upload_images/2960658-8dcc2e2a9e90480b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 没有配置环境变量,我们不能进入cy环境
![](https://upload-images.jianshu.io/upload_images/2960658-7e0b33d8936d5227.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 配置环境变量
![配置环境变量.png](https://upload-images.jianshu.io/upload_images/2960658-2a4e59501a69f19d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* 任何地方启动终端,就可以进入cy环境
![cy环境.png](https://upload-images.jianshu.io/upload_images/2960658-61e40c232afc7b4a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

这里就把mac系统Cy环境配置好了.

* 我们接下来安装iOS--Cycript

![Cycript](https://upload-images.jianshu.io/upload_images/2960658-64bfb613b52cd235.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 我们远程连接iOS终端

以百度外卖为例

![添加弹出框](https://upload-images.jianshu.io/upload_images/2960658-102d2bb525046f55.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![实现结果](https://upload-images.jianshu.io/upload_images/2960658-08c794a82dbc60ab.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


####11.theos
github地址:https://github.com/theos/theos
*   安装最新的theos
```
sudo git clone --recursive https://github.com/theos/theos.git /opt/theos
```
* 安装ldid(如安装theos过程安装了ldid，跳过)
```
brew install ldid
```
* theos使用
![theos使用.png](https://upload-images.jianshu.io/upload_images/2960658-8a7253a064e72151.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
在终端模式下,使用nic.pl,就可以创建tweak工程文件.

* 如果想在任意地方敲出nic.pl,就要配置环境变量

![配置环境变量.png](https://upload-images.jianshu.io/upload_images/2960658-91a39e7c818cf1cf.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* 环境变量配置好,以后使用起来会很方便的.
* 使用:
![nic.pl.png](https://upload-images.jianshu.io/upload_images/2960658-a8d0d5f15e9e56f4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

可以在终端中敲出nic.pl,
是在你环境变量配置好的情况下,
可以出现上面这个界面.
然后你就可以创建tweak项目工程了.
(这里不过多介绍,项目实战会介绍的)

####12.MonkeyDev
(注意:monkeyDev环境配置前,需要报theos环境配置好)
* 1.你可以通过以下命令选择指定的Xcode进行安装:
```
sudo xcode-select -s /Applications/Xcode.app
```
* 2.默认安装的Xcode为:
```
xcode-select -p
```
* 3.执行安装命令
```
sudo /bin/sh -c "$(curl -fsSL https://raw.githubusercontent.com/AloneMonkey/MonkeyDev/master/bin/md-install)"
```
* 4.卸载
```
sudo /bin/sh -c "$(curl -fsSL https://raw.githubusercontent.com/AloneMonkey/MonkeyDev/master/bin/md-uninstall)"
```
* 5.更新
```
sudo /bin/sh -c "$(curl -fsSL https://raw.githubusercontent.com/AloneMonkey/MonkeyDev/master/bin/md-update)"
```
安装/更新之后重启下Xcode再新建项目。

* 6.使用
安装成功后,打开xcode创建项目.你会发现呢?多了MonkeyApp选项
![MonkeyApp.png](https://upload-images.jianshu.io/upload_images/2960658-acfa14071a1b7952.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
这样,我们就可以创建项目了.

## 3.总结

工具安装和配置比较考验大家的动手能力,
配置好后,
它就是你最好的朋友.
这12款软件,
对于逆向开发必不可少,
就像一把锐利的工具,
打开了app的另一个世界.
还有很多帮助性的工具需要介绍,
今天就先介绍到这里,
文章会继续更新,
更多的软件使用也会写入文章,
请持续关注我的博客,
简书地址:https://www.jianshu.com/p/beea9f2b9f7d











