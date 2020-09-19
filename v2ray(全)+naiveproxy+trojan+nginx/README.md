注：

1、nginx为v2ray、caddy2(naiveproxy)、trojan(trojan-go)进行sni分流（四层转发），实现共用一个端口。

2、v2ray tcp类应用直连，v2ray WS类应用分流一次。

3、naiveproxy直连。v2ray h2类应用分流（反代）一次。

3、trojan(trojan-go)直连。
