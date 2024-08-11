# 基于Orangepi的大语言模型的简化工具链

<1>

首先 让我们假设你已经有了一块orange pi5Plus<这好像是废话>

<2>/////////////////////////////////////////////////////////

然后你需要下载并安装orangepi官方的 "Orangepi5plus_1.0.10_ubuntu_jammy_linux6.1.43"系统

地址:https://pan.baidu.com/s/1cQR1pcca0P-xuQbTrnGXAw?pwd=pjhv#list/path=%2F

建议选择server版本 系统占用内存相对小 方便我们运行大模型

<3>////////////////////////////////////////////////////////

然后下载并编译orangepi官方的6.1内核源码<这一步是为了更新一些驱动>

地址:https://github.com/orangepi-xunlong/linux-orangepi/tree/orange-pi-6.1-rk35xx
检查是否是 "orange-pi-6.1-rk35xx" 分支

将下载的包传至你的开发板 解压 然后根据项目文件里的 "" 文档操作

*如果你使用的是orangepi官方的散热器 是不是对官方那傻X散热策略感同深受?*
  *所以你可以使用我优化过的风扇驱动 就项目里那个 "rk3588-orangepi-5-plus.dts" 
将其放入下载的内核源码内的 "/arch/arm64/boot/dts/rockchip" 下覆盖掉原来的同名驱动文件即可
我实测即便高负载下风扇依然可以做到几乎无声 而温度却并没多大变化*

<4>////////////////////////////////////////////////////////

