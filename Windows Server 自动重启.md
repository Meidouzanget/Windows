# Windows
收集一些Windows的智障小问题

##### 某一天远程发现我的桌面的和昨天不一样了，查看CPU运行时间在凌晨5点重启过。

吓得我以为机器被黑了。因为Windows server 默认是不会自动重启的，并且也设置了手动更改更新

事件管理器查看系统日志，发现了以下纪录

    进程 C:\WINDOWS\system32\svchost.exe (WINSERVER-PUBLI) 由于以下原因已代表用户 NT AUTHORITY\SYSTEM 启动计算机 WINSERVER-PUBLI 的 
    重启: 操作系统: Service Pack (计划内)
     原因代码: 0x80020010
     关机类型: 重启



![image](https://user-images.githubusercontent.com/59044398/226078030-b8e85a4f-8493-4724-9264-29c836f66bd8.png)


在微软技术支持网站上找不到事件ID为1074的解释记录。在查询原因代码0x80020002时，发现两篇文章提到了这个问题：

　　一篇微软的技术人员Tim Rain的　 Is Windows Automatic Update Client rebooting your system unexpectedly? Read this to “fix” it…
  
　　虽然他说提XP应用，但是对服务器版本也应该同样适用的。可以断定的是，是因为Windows Automatic Update服务惹的祸，微软发布了几个升级补丁。因为它导致了不可预期的重启动。

如果不想让系统自动重启，选择第二项“下载更新，但是由我来决定什么时候安装。”就可以了。
 
 
    1.依次选择“计算机右键属性→高级系统设置→性能和维护→系统”，打开“系统属性”对话框。
    2. 选择“高级”选项卡，在“启动和故障恢复”下，单击“设置”按钮。
    3. 在“系统失败”下，取消勾选“自动重新启动”复选框，单击“确定”按钮

![image](https://user-images.githubusercontent.com/59044398/226078212-f490c765-2ced-4352-92f2-3d03fc012864.png)





PS:


https://blog.csdn.net/levy_cui/article/details/51140924


https://learn.microsoft.com/zh-cn/windows/deployment/update/waas-restart

https://blog.csdn.net/GHY2016/article/details/88889700


