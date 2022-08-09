# 总结

[参考链接](https://www.raspberrypi.com/news/coding-on-raspberry-pi-remotely-with-visual-studio-code/#:~:text=Select%20the%20Extensions%20tab%20from,%2BShift%2BP%20on%20macOS.)

远程开发，只需供电，极大地提高了开发的灵活性。


# 教程

硬件需求：树莓派3或4代；大于15W的Type-C充电器；一张sd卡；路由器。

安装时还需要：USB键盘；显示器；有一端为miniHDMI接口的HDMI线；可以刻录镜像文件至sd卡的设备（如一台Windows电脑+读卡器）。

去[树莓派官网](https://www.raspberrypi.org/)下载系统镜像，推荐64位LiteOS。根据官方指引刻录系统至sd卡。

初始化后使用raspi-config连接Wifi。

通过路由管理页面获取ip地址，建议在路由中设置DHCP固定IP地址。

此时回到主力机，树莓派可以断开所有外设。打开VScode，左下角Open a Remote Window -> Connect Curren Window to Host -> add ssh config -> 输入user@ip -> 输入密码 -> 配置完毕。