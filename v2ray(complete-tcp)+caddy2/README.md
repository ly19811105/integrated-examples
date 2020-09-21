注：

1、除v2ray kcp外,所用应用共用443端口。此端口由caddy2监听，caddy2前置，反向代理分流ws与h2。无vless tcp应用。

2、v2ray ws类应用分流（反代）一次。v2ray h2类应用分流（反代）一次。

3、caddy2 等于或大于v2.2.0-rc.1版才支持反向代理v2ray H2(HTTP/2) 应用。
