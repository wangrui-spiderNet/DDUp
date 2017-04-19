# DDUp
DDUP设计


1、adb logcat 　　　　　　　　  --打印当前设备上所有日志

2、adb logcat | findstr ***　　 --过滤仅含***的日志

3、adb logcat *:W 　　　　　　 --过滤打印严重级别W及以上的日志

4、adb logcat | findstr *** > F:\log.txt 　　 --把仅含***的日志保存到F盘的log.txt文件中

5、adb logcat -c 　　　　　　    -- 清除屏幕上的日志记录

6、adb logcat -c && adb logcat -s ActivityManager | grep "Displayed”  　　--客户端程序启动时间获取

查看当前Activity
Windows :
adb shell dumpsys activity | find "mFocused"

MAC:
adb shell dumpsys activity | grep mFocused 


cmd常用控制台
1、清屏命令：cls
2、列出当前目录详细信息：dir
3、删除文件：del xxx.txt


android adb常用命令
1)、创建sdcard
mksdcard 50M D:/sdcard.img --> 创建一张容量为50M的SDCard

2)、删除sdcard
cd d:/
del sdcard.img

3)、把ljq.txt文件放在sdcard
adb push d:/ljq.txt /sdcard/

4)、创建avd模拟器
android create avd -n avd名称 -t target平台编号
eg、android create avd -n android2.1 -t 8

说明：Error: Folder C:\Users\Administrator\.android\avd\ljq.avd is in the way. Use --f
orce if you want to overwrite.(进入C:\Users\Administrator\.android\avd\目录，把ljq.avd文件夹删除即可)

5)、启动模拟器
emulator -avd xxx
eg、emulator -avd android2.1
启动带sdcard模拟器
emulator -sdcard d:/sd.img -avd android2.1(android2.1之前创建好的一个虚拟设备的名称)

6)、删除AVD（模拟器）：
android delete avd -n name名称
eg、android delete avd -n android2.1

7)、显示系统中全部android平台
android list targets

8)、android list avd 

9)、adb devices

10)、查看用户已安装的软件
adb shell
cd /data/app/ 
ls

11)、安装软件
adb install d:\abc.apk

12)、卸载软件
adb shell
cd /data/app/
adb uninstall <软件名> 
adb uninstall -k <软件名> 
说明：如果加 -k 参数,为卸载软件但是保留配置和缓存文件. </B>
eg、adb uninstall com.ljq.activity

13)、启动ddms：ddms

14)、导出文件
adb pull adb pull <远程路径> <本地路径>  
eg、adb pull /sdcard/hrtx/123.gif d:/

15)、导入文件
adb push <本地路径> <远程路径>
eg、adb pull d:/123.gif /sdcard/

16)、进入模拟器的shell模式：
adb shell

17)、在命令行中查看LOG信息：
adb logcat
adb logcat -s 标签名
eg、adb logcat -s MainActivity

18)、删除系统应用：
adb remount(重新挂载系统分区，使系统分区重新可写)
adb shell
cd /system/app
rm *.apk

19)、获取管理员权限：
adb root

20)、启动Activity
adb shell am start -n 包名/包名＋类名(-n 类名,-a action,-d date,-m MIME-TYPE,-c category,-e 扩展数据,等)
eg、adb shell am start -n com.hrtx.activity/com.hrtx.activity.MainActivity

21)、发布端口： 
设置任意的端口号，做为主机向模拟器或设备的请求端口。
eg、adb forward tcp:5555 tcp:8000 

22)、查看bug报告： 
adb bugreport 

23)、记录无线通讯日志： 
一般来说，无线通讯的日志非常多，在运行时没必要去记录，但我们还是可以通过命令设置记录： 
adb shell 
logcat -b radio 

24)、获取设备的ID和序列号： 
adb get-product 
adb get-serialno 

25)、访问数据库SQLite3 
adb shell 
sqlite

==================================================================================================================================
