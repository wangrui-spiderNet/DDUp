# DDUp
DDUP设计
前身
巨变
秘密
转化


主线：
科技危机，科技的生长脱离的多数人的掌控后

更先进不代表更强大

副线：
科技的发展对人类社会的巨大影响，科技的残酷，不同阶层人类面对巨变的命运
人类对自由的渴求，对永生的渴求，对成为神的渴求
人没有善恶，只是立场处境不同而已
生命的意义到底为何?
真实的人工智能到底是会怎么样？
政府的角色？
科技竞赛如果脱离了政府的掌控？
高科技公司的演变
战争还是和平？
不能调和的矛盾
越来越大的差距
富者永生，穷者无助
时间的不平等
身体的差异
高等级的人与低等级的人
如何重新定义人
不能改变的现实-人性（自私，欲望，绝对自由，绝对的孤独，无上的权力，恐惧）
暂时的困境
过渡期会怎么样发生？
新的世界会如何到来？
人类的潜力到底有没有边界？
进化的代价
得到什么，失去什么？
科技的原始驱动力是什么？邪恶还是好奇？欲望和懒惰还是聪明的大脑
一切都在改变，唯有人性未变
选择
更“好”的人，普通人？
改变了的人性还是人吗？

智人和半超人


剧情转换：
巨变，重生，进化，新的朋友，两种人，另一个世界，阴谋，背后的背后，巨变，
逃离，变强，自由，责任，路在何方


主要情绪：
科技的冰冷
无助
恐惧
残酷
邪恶
金钱
战争
交易
力量
兴奋
亲情
抚慰
自由


原则：
大胆猜测，仔细构想

像在讲述过去一样讲述未来

先想象一下一百年以后会是怎么样一个社会，然后倒退从现在走向未来100年中间会发生什么

满足普通人对未来的窥探，对科技发展的好奇

===========================================================================
智远集团首席科学家  王安  他的儿子 王栩然 小天才

故事主线：
第一部分：
平静的生活突然有一天出现了崩塌，全家失散，城市陷落，人们流离失所，只有自己的小机器人还在身边陪伴，为了弄清楚这到底是怎么回事，找到父母，主人公开始一段探索，随着探索的深入揭露出了一个惊人的秘密，原来这一切的发生都不是突然发生的，一个超级庞大和黑暗的组织开始出现，主人公开始了一段与超级巨鳄斗争之旅。


第二部分：
当超级巨额的面目一步步更加清晰的时候，一个更大的阴谋和谎言开始出现，他的父母的身份让人怀疑，他自己又是谁？
他只是一对科学家（他的父母）的研究成果而已，而过去的种种也只是整个实验的一部分，真实的世界远不是这样。他该怎么办，按照设定的命运走向垃圾场，还是争取自己的生存权利？在父母的帮助下，他活了下来。
他，一个机器人，被人类创造出来的人，面对人类的设定会做出什么样的选择？他超乎普通人类的能力在面对脆弱的真实人类的时候，当他已经主宰了自己的命运，还有能力主宰全人类的命运的时候，他会怎么做？


第三部分：这只是一个实验。

实验的完整版图
第一阶段：培养
第二阶段：接受考验，判别是非的能力测试，面对恶劣的环境的生存能力测试
第三阶段：探索真相，接受现实，精准的反抗测试，当接受自己是机器人之后，他要为了生存而抗争，当经受人类的摧残和恶意，生存下来并强大之后，能够依然保持对人类和世界的热爱。
第四阶段：实验结束，实验结论，机器人是可信的，通过测试，可以批量生产进入人类社会。


第四部分：觉醒。

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
