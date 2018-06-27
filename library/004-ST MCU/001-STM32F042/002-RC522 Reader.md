# M1 Card Reader

一款可以对M1卡进行读写的设备，下位机是STM32F042+RC522模块，使用USB通讯，上位机使用QT+libusb

### 下位机

### 上位机
下面演示了
* 查找设备，选择rc522 reader,打开设备
* 获取卡片，这一步骤包含了寻卡、防碰撞、选卡，并显示了测试卡片的UID
* 验证密匙
* 演示了对块进行读取、写入

![alt文本](amWiki/images/rc522/M1 Card Reader.gif "RC522 reader")

### 其他

详细信息请查看

下位机及上位机查看github
