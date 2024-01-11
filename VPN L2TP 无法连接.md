#### 错误1：解决WIN10 vpn 连接错误 “无法建立计算机与VPN服务器之间的网络连接,因为远程服务器未响应。”

![image](https://github.com/Meidouzanget/Windows/assets/59044398/1ebf791f-45d8-41bf-8882-2401c71ae4ef)

1.打开注册列表，进入 HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\PolicyAgent

2.在右边空白处新建 > DWORD值”，名称为AssumeUDPEncapsulationContextOnSendRule

![image](https://github.com/Meidouzanget/Windows/assets/59044398/ec18738f-e4d6-47ae-b85c-7a5cd6a708d4)

3.双击“AssumeUDPEncapsulationContextOnSendRule”，修改值为2(表示可以与位于NAT设备后方的服务器建立安全关联)

![image](https://github.com/Meidouzanget/Windows/assets/59044398/1e9b7430-6617-4018-86f1-0eaedf6e030c)

4.重启电脑


#### 错误2：修改完注册表，错误就变了，是因为认证的协议问题

![image](https://github.com/Meidouzanget/Windows/assets/59044398/59b01a33-4a12-4c39-ab64-f985541f3f23)

1.打开WLAN设置-->网络共享中心-->更改适配器设置

![image](https://github.com/Meidouzanget/Windows/assets/59044398/cce38a19-f946-4de2-b96a-6c7c54297e72)

![image](https://github.com/Meidouzanget/Windows/assets/59044398/be272a56-130c-4035-8bc9-9738d4b439b2)

2.选择你L2TP VPN，右键属性

![image](https://github.com/Meidouzanget/Windows/assets/59044398/7ba93f18-9be0-4227-ac23-d71b76952c98)

启用允许这些协议，勾上你设置的协议。比如我用的是群晖VPN Server设置了 MS CHAP V2.当然全部勾上也不是不行

![image](https://github.com/Meidouzanget/Windows/assets/59044398/35a2d0bc-f496-486c-ad86-c799df567121)

3.连接成功

![image](https://github.com/Meidouzanget/Windows/assets/59044398/428d5581-9bc9-4e04-9819-04933fab59fb)



