注：

1、除v2ray kcp外,所用应用共用443端口。此端口由v2ray监听，v2ray前置。利用vless tcp回落/分流特性实现。

2、v2ray tcp类应用直连。v2ray WS类应用分流一次。v2ray h2类应用回落一次，分流（反代）一次，共计两次。

3、caddy2 等于或大于v2.2.0-rc.1版才支持反向代理v2ray H2(HTTP/2) 应用。
