### 1、在终端里 apt-get安装的软件：
安装软件sudo  apt-get install softname1 softname2softname3……  
卸载软件 sudo apt-get remove softname1 softname2 softname3……  
卸载并清除配置sudo  apt-get remove --purgesoftname1  
更新软件信息数据库 sudo apt-get update  
进行系统升级sudo  apt-get upgrade, sudo apt-get distupgrade  
搜索软件包 sudo apt-cache search softname1 softname2 softname3……  

### 2、安装的deb包要用此方法：
安装deb软件包 dpkg -i xxx.deb  
删除软件包 dpkg -r xxx.deb  
连同配置文件一起删除 dpkg -r --purge xxx.deb  
查看软件包信息 dpkg -info xxx.deb  
查看文件拷贝详情 dpkg -L xxx.deb  
查看系统中已安装软件包信息 dpkg -l  
重新配置软件包 dpkg-reconfigure xxx  

### 3、在“synaptic pakagemanager”里:
点搜索，输入软件名  
在需要安装或卸载的软件上右击－点标记－最后点应用  

### 4、现在还可以在 software center里面,直接卸载。

### 5、卸载源代码编译的的软件：
cd 源代码目录  
make clean  
./configure  
（make）  
make uninstall  
rm -rf 目录  

清理系统：  
sudo apt-get autoclean  
sudo apt-get clean  
sudo apt-get autoremove  
（或使用ubuntu-tweak清理）  

### 6.Linux下改变启动器（状态栏）位置命令：
底部：gsettings set com.canonical.Unity.Launcher launcher-position Bottom  
左侧：gsettings set com.canonical.Unity.Launcher launcher-position Left  

### 7.进入或返回上下层级目录：
进入下一层级：cd 目录名  
返回上一层级：cd ..  
返回上两层级：cd ../..  
返回根目录：  cd或cd ~  
