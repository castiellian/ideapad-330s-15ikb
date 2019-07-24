# ideapad-330s-15ikb

[config] 联想Lenovo ideapad 330S 15IKB 美版笔记本Mac Catalina 完美99%

美国walmart 入的廉价版笔记本，联想Lenovo ideapad 330S 15IKB 美版


配置如下：

CPU：i5-8260U

主板：Intel Kaby Lake-U + iHDCP 2.2 Premium PCH

显卡：Intel UHD Graphics 620

内存： DDR4 2400 8G

SSD1：海康威视C2000 256GB NVME SSD（win10+macOS Mojave）

SSD2：HP 海力士 1.92TB SATA SSD （DATA+macOS Catalina+PhoenixOS+DeepinLinuxOS）

Wi-Fi：DW1820A（BCM94350ZAE）带蓝牙BCM2045A0 (Device id: VendorID/ProdoctID=0x0a5c/0x6414)

有线网卡：CE-Link USB 有线网卡

显示器：京东方  1920x1080P 60HZ

1,   安装系统之前，先对笔记本bios 升级到最新版：7SCN28WW

2，使用insyde  H20UVE工具对bios 的DVMT 占用内存设置为64MB

将文件H20UVE 放到C盘或者D盘。

然后cmd 管理员运行：

cd C:/H20UVE/ 
H20UVE.exe -sv 330s.txt 
(330s.txt 包含修改好insydeh20 bios 设置参数，可将DVMT 内存设置为64mb，就可以不用打核显DVMT Framebuffer二进制补丁)


3, 将我的配置文件Clover放到EFI分区，安装系统。

注意：安装Catalina时，用我里面的安装专用kext，安装进入系统后，将我的配置kext复制到kext文件夹，修复系统权限。

