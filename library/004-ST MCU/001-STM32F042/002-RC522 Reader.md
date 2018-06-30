# M1 Card Reader

一款可以对M1卡进行读写的设备，

### 下位机

下位机是STM32F042+RC522模块，还有个指示LED灯、蜂鸣器，使用USB通讯，如下图：

正面：

![alt文本](amWiki/images/rc522/rc522_4.jpg "RC522 reader")

USB接口：可以看到很大一个孔，外壳原来留的孔是用于USB A接口的，我用的是micro USB接口

![alt文本](amWiki/images/rc522/rc522_3.jpg "RC522 reader")

里面：可以看到STM32F042模块、RC522模块、红色的二极管灯、蜂鸣器模块，还有接出来的4PIN排针用于调试

![alt文本](amWiki/images/rc522/rc522_1.jpg "RC522 reader")

### 上位机
上位机使用QT+libusb

下面演示了
* 查找设备，选择rc522 reader,打开设备
* 获取卡片，这一步骤包含了寻卡、防碰撞、选卡，并显示了测试卡片的UID
* 验证密匙
* 演示了对块进行读取、写入

![alt文本](amWiki/images/rc522/M1 Card Reader.gif "RC522 reader")

### 其他

下位机及上位机查看[github](https://github.com/halin-Lab/STM32F042/tree/master/software/RC522)
