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




















