# Cube i7 Stylus Hackintosh
酷比魔方i7手写版自己日常使用的 CLOVER 配置文件

## 说明
目前支持10.14.4，无法正常升级系统需要更新 clover 版本

除了蓝牙和读卡器外其他全部驱动，基本满足日常使用

一些小问题会在以后修复

## 使用
### BIOS
- 开机按 ESC 进入 BIOS  
- Advanced -> CPU Configuration -> Limit CPUID Maximum -> Disabled  
- Advanced -> CPU Configuration -> Execute Disable Bit -> Enabled  
- Advanced -> CPU Configuration -> Intel Virtualization Technology -> Disabled  
- Advanced -> CPU Configuration -> CFG lock-> Disabled  
- Chipset -> System Agent (SA) Configuration -> VT-d -> Disabled  
- Chipset -> System Agent (SA) Configuration -> Graphics Configuration -> DVMT Pre-Allocated -> 128M  
- Boot -> Bootup NumLock State -> Off  
- Save & Exit -> Save Changes and Reset  

### CLOVER
1 备份并删除 /EFI/CLOVER  
2 下载本仓库并重命名文件夹为“CLOVER”  
3 把 CLOVER 移入 /EFI/  
4 Clover Configurator 打开 config.plist -> 机型设置，重新生成 smbios  

## 工作
- 显卡  
- 声卡  
- 网卡  
- Wi-Fi  
- USB  
- 触摸屏  

## 不工作
- 蓝牙  
- 读卡器  

## 待解决问题
- 重启不断电  
- USB 3.0 速度 480MB  
