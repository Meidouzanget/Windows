# Windows
收集一些Windows的智障小问题

开始---运行---输入regedit.exe,启动注册表编辑器，
打开HKEY_CURRENT_USER\Software\Microsoft\Windows\ CurrentVersion\Policies\Explorer子项

在Explorer子项中如果有一个名为NoNetConnectDisconnect的双字节值项

如果该值项的数值数据为1的则把文件删除

重启电脑后验证
