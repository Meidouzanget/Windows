# Windows
收集一些Windows的智障小问题

### 首先

检查安全中心的防火墙出站入站设置

有些装了杀毒软件的这里会显示灰色

![image](https://user-images.githubusercontent.com/59044398/200111542-4c59d294-975b-4529-a401-8af65f30c442.png)

像 eset 这里罗技就被阻止了

![image](https://user-images.githubusercontent.com/59044398/200111600-97afd292-4aac-4d43-a769-38a0ac49239a.png)


![image](https://user-images.githubusercontent.com/59044398/200111514-ace60201-a608-4ca6-8375-b20870931c97.png)

### 第二

检查网络是否能 ping 通，如果 ping 不通，可能是因为公共网络安全设置不允许

设为专用网络

![image](https://user-images.githubusercontent.com/59044398/200112267-153ad927-29f4-420a-b135-a6118d551cb3.png)




### 第三

如果还是不行，检查出站入站设置，虽然我也没测试过删了还行不行，出站是默认没有的，后来加的

找到LogiOptionsMgr.exe，在入站复制路径，新增一个到出站

![image](https://user-images.githubusercontent.com/59044398/200112492-6dec7ebd-d6f9-48bd-bf19-2264f4fb1da4.png)


![image](https://user-images.githubusercontent.com/59044398/200112356-045c51e7-e6bd-405c-a83b-6a3fa15f294a.png)

![image](https://user-images.githubusercontent.com/59044398/200112416-9a806cea-cb83-44fc-8dff-53916c96aabd.png)

![image](https://user-images.githubusercontent.com/59044398/200112452-cb4ab684-c4fe-4435-9a28-0f33eb9294bb.png)

### 第四

还是不行，那就最后一步

根据罗技官网所述，在路由器添加端口

![image](https://user-images.githubusercontent.com/59044398/200112564-68171541-75dd-4754-b010-c041b2193e0b.png)

![image](https://user-images.githubusercontent.com/59044398/200112624-8ebb3ddf-30d2-4f15-ab39-5361e596c433.png)

启用并添加通信端口触发程序。

应用设置，并重启路由器

![image](https://user-images.githubusercontent.com/59044398/200112784-b931e83c-4be9-46df-81ad-56f929454fcc.png)



