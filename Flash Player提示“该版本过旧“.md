# Windows
收集一些Windows的智障小问题

1. 打开路径,复制host文件到桌面
```
C:\Windows\System32\drivers\etc
```

2. 在host中写入一规则
```
127.0.0.1 geo2.adobe.com
127.0.0.1 fpdownload2.macromedia.com
127.0.0.1 fpdownload.macromedia.com
127.0.0.1 macromedia.com
```

3. 运行命令刷新规则
```
ipconfig /flushdns
```

4. 如果之前运行过abode flash player，且无法回滚系统，则需要删除流氓的缓存
```
用Everything搜索：Shockwave Flash 文件夹，全部删除，（若不存在此文件夹则跳过）
用Everything搜索：Macromedia 文件夹，全部删除，（若不存在此文件夹则跳过）
```

5. ping 一下上面的地址，如果返IP为 127.0.0.1，则设置成功。

   エロゲーム　起動‼

   あああ 犬姫は超可愛い～


   



