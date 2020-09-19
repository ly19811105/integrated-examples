注：

1、v2ray、caddy2(naiveproxy)、trojan(trojan-go)各自监听一个端口，分别或配合提供服务。如caddy2为v2ray、trojan(trojan-go)提供回落服务。

2、v2ray tcp类应用直连，v2ray WS类应用分流一次。

3、naiveproxy直连。v2ray h2类应用分流（反代）一次。

3、trojan(trojan-go)直连。
