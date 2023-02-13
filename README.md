## 部署

* 注册 [Deepnote](https://deepnote.com/)
* 创建一个Project，点击Environment中的Initialization，打开里面的`init.ipynb`
* 删除里面自带的代码块并创建一个，输入下面的内容

```
!sleep infinity
```

![](https://gcore.jsdelivr.net/gh/Misaka-blog/imgs@main/20230208164251.png)

* 打开 Allow Incoming Connections 的开关
* 在命令行复制粘贴，运行以下命令中的其中之一

Vmess: 

```shell
wget -N https://raw.githubusercontent.com/Misaka-blog/v2ray-for-deepnote/main/deep.sh && bash deep.sh
```

Vless:

```shell
wget -N https://raw.githubusercontent.com/Misaka-blog/v2ray-for-deepnote/main/deep-vless.sh && bash deep-vless.sh
```

* 节点配置如下

```
协议：Vmess / Vless
地址：xxxxx.deepnoteproject.com
端口：443
UUID/密码：8d4a8f5e-c2f7-4c1b-b8c0-f8f5a9b6c384 或自己定义的UUID
额外ID：0
传输协议：ws
伪装域名：xxxxx.deepnoteproject.com
路径：/
传输安全：TLS
跳过证书验证：true或false都可以

