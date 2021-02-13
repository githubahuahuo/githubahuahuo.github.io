#安卓刷机  

**刷机步骤**:  
①**解锁**，注意是bootloader锁，不是id锁（某些厂商还需要申请解锁码才可以）(https://www.miui.com/thread-10101861-1-1.html)

②**刷第三方REC** 

前言    
一、recovery  
 recovery翻译成中文的意思是”恢复“，一般我们会简称为REC，recovery是一个可以对安卓机内部的数据或系统进行修改的模式，类似于windows PE或DOS。MIUI目前内置了一个功能比较单一的REC，本期主要讲讲如何刷入三方recovery，解锁更多功能。     

二、twrp    
twrp是由teamwin以及omni开源的第三方recovery，全名是：TeamWin Recoverytwrp是由teamwin以及omni开源的第三方recovery，全名是：TeamWin Recovery Project。TWRP的主要作用包括刷机，备份，恢复等1。通过编译适配，可以让大多数的手机/平板用上该recovery，该recovery的最大特点就是支持触屏，界面友好，功能强大，是刷机不可缺少的工具。    

三、LR.Team定制版TWRP  
 LR.Team是由熟悉制作安卓Rom和REC的开发人员组成的非盈利性团队，本期主要用前MIUI论坛呵呵105适配的recovery作为教程，他跟微博“Wz5x150”是同一人，W大已为小米50余款机型适配定制版TWRP，目前他主要在微博更新，后续可能会入驻新社区。 
 
**教程**  
TWRP（Team Win Recovery Project）是一款非常强大的Recovery刷机工具。刷机有风险，操作之前请备份重要数据。  

方法一： fastboot刷TWRP   
	去TWRP官网下载TWRP安装文件https:/twrp.me/Devices/
选择你需要刷入TWRP的设备，然后下载相应的刷机文件，比如选择的是Xiaomi Mi 5， twrp-3.5.0_9-0-gemini.img.
	根据您的操作系统下载SDK平台工具[platform-tools](https://developer.android.com/studio/releases/platform-tools)
Windows 操作系统下的 ADB 环境配置

1.进入fastboot
在控制台下进入已下载TWRP刷机包的目录，键入命令：adb reboot bootloaderadb reboot bootloader 也可在开机时，同时按住电源键+音量减，进入fastboot（不同的手机进入方式稍微有所差别）

2.输入以下指令
输入：adb devices（手机确定允许adb调试）  
输入：adb reboot bootloader（进入fastboot模式）  
输入：fastboot devices（若出来一串序列号，说明安卓设备已连接）  
输入：fastboot flash recovery xxx.img（直接拖动镜像文件到cmd，避免找不到路径）  

3.刷入成功后，拔掉手机的USB数据线，进入TWRP recovery。一般来说，进入recovery有三种方法：  
	adb命令进入recovery模式，执行以下命令：adb reboot recovery  
	在关机的状态下，按下厂商设定的组合键，每台手机可能不一样，（小米 电源键+音量加键）  
	在Bootloader下，用降低音量键定位到Recovery，按下升高音量键或电源键确认，你的手机应该会重启到recovery   

方法二：app安装方法

下载官方TWRP应用程序Official TWRP App（需要root）  
下载TWRP Manager.apk后安装，首先授予Root权限，然后选择自己设备后会自动下载相应刷机包，根据提示进行操作即可。  

[TWRP官方网站](https://twrp.me/) 
[橙狐REC官方网站](https://sourceforge.net/projects/orangefox/files/)
[LR.Team修改版 覆盖大部分机型 ](https://t.me/xiaomi6666/43584)  
（如果没有你的机型REC，可以尝试去酷安、MIUI论坛、xda论坛，谷歌找找）  

③**在twrp中安装你想要使用的刷机包**  
原厂系统第一次刷第三方系统 ，建议在清除里格式化data分区（会清空手机存储）一遍再刷系统，减少不确定因素的影响。注意格式化data分区后需要重启，然后重新进入rec，由电脑导入刷机包，然后刷机

原生系统  
[AEX](https://downloads.aospextended.com/)   
[pixel](https://download.pixelexperience.org/)    
[lineageos](https://download.lineageos.org/)   
[魔趣](https://download.mokeedev.com/)    
[havoc](https://sourceforge.net/projects/havoc-os/files/)   
[RR](https://get.resurrectionremix.com/)  
[omni](https://www.omnirom.org/)  
[dotOS](https://www.droidontime.com)  
[GrapheneOS](https://grapheneos.org)  
[AOSP](https://www.aospextended.com/)  
[syberia](https://syberiaos.com/downloads)  
[RevengeOS](https://download.revengeos.com/)  
[Evolution-x](https://evolution-x.org/)  

[XDA ROM交流论坛](https://www.xda-developers.com/)  

其他版本MIUI:  
[欧版](https://xiaomi.eu/community/threads/20-7-2.56447)）  
[波兰版](https://miuipolska.pl/download/)  
[国际版](https://c.mi.com/miuidownload/index)  

视频教程  
