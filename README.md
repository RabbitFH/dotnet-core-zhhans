>汉化前 :    

![image](imgs/01%20%E6%B1%89%E5%8C%96%E5%89%8D.png)    

> 汉化后 :    

![image](imgs/03%20%E6%B1%89%E5%8C%96%E5%90%8E.png)    

---
# 注意 ！！！！！！！！！！！
 **百度翻译2022-8-1日起调整免费版权益，调用API每月超过5W字符后开始计费**   
为避免产生费用，可在lastReleases目录中下载最新的打包文件，并且关闭百度api！   
如有其它的免费API，欢迎分享！   

# 下载
> 2.0.0 以下版本需要手动更新！    

下载链接 : [url](http://www.wyj55.cn/DotNetCoreZhHans.html) 或 lastReleases目录中下载最新的打包文件。
内置数据库已包含常用库的翻译数据，可以离线翻译。
建议注册百度翻译API账号 注册地址:`（不是“百度云下”的翻译，是“百度翻译”！！！！！）` https://fanyi-api.baidu.com/    
到“开发者中心”>“开发者信息”拿到“APP ID”和“密钥” ，然后进入“配置”> “API选项” ，填写参数。Secretld 填  APP ID , SecretKye 填 密钥。更新如果遇到问题，请删除\lib\DotNetCorezhHansMain.exe，重新打开即可。

> 要求x64系统，并且安装.NET6！

---

# .NET Framework 项目
请将 “packages.config” 迁移到 “packagesReference”之后可用，在当前项目 "引用" 上点右键进行迁移。    
![image](imgs/02%20NET%20Framework%20%E9%A1%B9%E7%9B%AE%E8%BF%81%E7%A7%BB.png)

---    

# 使用    
![image](imgs/%E4%BD%BF%E7%94%A8.gif)    

---    

# API选择

提供商  | 单次最大请求 | QPS | 每月免费额度 | 免费额度超出后果
---  |  --      | --    | --        | --
百度 |  1000    | 1     |   5W      | 收费
腾讯 |  2000    | 5     |   500w    | 停止服务
阿里 |  5000    | 50    |   100w    | 计费
华为 |  2000    | 未知  |   100w    | 计费
---

# 关于翻译中的”异常”
异常并不代表整个文件不可用，而是某些行没有通过严格的检查，这些错误要么来自翻译引擎，要么是软件代码原因，以超大文件netstandard.xml为例，大约会出现10个异常。出现异常的内容不会写入数据库，等以后能解决的时候开启“重新生成”即可。

---

# 常见问题
1.	扫描中必须有对应的同名dll文件，否则被忽略。
1.  如果XML文件中包含阿拉伯文字，会被忽略。
1.  如果更新.NET自带的XML文档，需要开启管理员权限，否则出现错误” is denied”。

---

# 建议扫描路径
```
%UserProFile%\.nuget\packages\
C:\Program Files\dotnet\packs\
C:\Program Files (x86)\Microsoft SDKs\
C:\Program Files\Microsoft Visual Studio\2022\Community\Common7\IDE\ReferenceAssemblies\Microsoft\Framework\
客户端需要升级到2.0.0版本，否则会出现意外退出现象。
```

---

# .NET官方汉化包
在官方汉化包的基础上，加个了个小程序自动拷贝。   
[下载](http://www.wyj55.cn/download/DotNetCorezhHans/Dotnet-Intellisense1.0.0.0.7z)

---

# 由于英语水平问题，所以不要纠结源码中的命名！
> 不然我干嘛写这个？ ^__^      
---
# 免责声明
本软件为免费提供，源码根据开源协议提供，本人不承担使用软件或源码导致的任何后果。