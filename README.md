火狐浏览器在window和Linux下可以使用同一账号登录，同步书签很方便。但是Ubuntu16.04自带火狐不是中文版，看起来不方便而且不能和中文版同步。
1.下载最新版本：http://www.firefox.com.cn/
2.删除自带的国际版火狐浏览器，打开终端输入：
  sudo apt-get remove firefox
3.将下载好的压缩包解压，解压出来的文件夹名为firefox，将其移动到/opt目录下，输入：
  sudo mv firefox /opt
4.进入目录：
  cd  /usr/share/applictions
5.创建firefox.desktop文件：
  sudo touch firefox.desktop
6.编辑内容：
[Desktop Entry]
Name=firefox
Name[zh_CN]=火狐浏览器
Comment=火狐浏览器
Exec=/opt/firefox/firefox
Icon=/opt/firefox/browser/icons/mozicon128.png
Terminal=false
Type=Application
Categories=Application
Encoding=UTF-8
StartupNotify=true
7.保存后重启：
sudo reboot
8.在dash下搜索Firefox就可以找到我们安装的中文版火狐浏览器。
