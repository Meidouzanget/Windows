# Windows
收集一些Windows的智障小问题

#### 最近播放视频不知怎么变得卡了起来，以为是Windows 远程的问题，搞了一通发现是PotPlayer更新后有些设置改变了或是没做好。Windows也是这样更新之后注册表的设置被更改了什么的....

#### Mad 和 LAV

因为我的设置是沿用之前的实体机的，发现远程虚拟机 Mad 和 LAV 都不能用，无论怎样设置。即使配置了GPU也没用

具体表现为占用极高，播放卡死，拖动进度条立马暴毙

所以这里有关Mad 和 LAV的东西全部关闭改为默认

![image](https://github.com/Meidouzanget/Windows/assets/59044398/81696b31-b31b-4466-8a55-9eac87d52ccc)

设置开启

![image](https://github.com/Meidouzanget/Windows/assets/59044398/a59d865c-4a2a-4ab3-9153-bd7f381c71a1)

滤镜全部不要勾

![image](https://github.com/Meidouzanget/Windows/assets/59044398/4831e14f-9d92-4b56-907a-8169fe21ea71)



#### 这里设置了Ditect3D 11 和选择了GPU后，流畅了一点

![image](https://github.com/Meidouzanget/Windows/assets/59044398/37e86e44-6eff-419f-ba1d-c301ff5c25bd)



#### 设置完下面的就完全不卡了

这里的选项是对应GPU 的Video Decode，如果发现播放视频这里无活动那就是出问题了。这里设置之前播放一直是卡的

![image](https://github.com/Meidouzanget/Windows/assets/59044398/b26ee3a6-dee3-4b8d-ac06-b53863140ad1)


![image](https://github.com/Meidouzanget/Windows/assets/59044398/ff1de73a-8e92-4b21-88d2-35a9140af890)


####################################################################

没有动设置，第二天播放突然就变卡了，遗留的窗口再重新连接远程桌面会导致问题。
观察到如上图，Video Decode没有活动。
关掉所有potplayer窗口再启动恢复正常。
 

####################################################################
发现一个MKV视频有音画不同步，其他都没问题，属性查看是个AVC1 
![image](https://github.com/Meidouzanget/Windows/assets/59044398/5c3d2f31-b2cf-4080-a536-4e1e2184ed53)

台式电脑是没问题的，又是远程机不行，尝试安装台式的配置安装LAV

配置参考：https://blog.csdn.net/ronghua189/article/details/124522236


这里原用这里Direct3D 11，可以改为OpenGL 或 Madshi
![image](https://github.com/Meidouzanget/Windows/assets/59044398/9498aee6-8bc7-44db-bffd-8a904ed15d7f)

这里用默认GPU占用会比较多，Video Decode有活动；用LAV则CPU占用比较；Video Decode无活动。

![image](https://github.com/Meidouzanget/Windows/assets/59044398/6d439d14-95fb-4541-b969-0f342f62c34d)

![image](https://github.com/Meidouzanget/Windows/assets/59044398/2a263a86-c115-4875-a4a4-e95fc5fd6ae1)

![image](https://github.com/Meidouzanget/Windows/assets/59044398/7e227c67-68cb-45eb-ac80-35c5eb497ba3)

后来结合和LAV又试了一下MadVR，播放时正常的但有点有点时间回溯的样子，画面偶尔前后震荡。补帧负优化，补了个寂寞






