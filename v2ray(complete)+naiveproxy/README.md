注：

1、除v2ray kcp外,所用应用共用443端口。此端口由v2ray监听（即v2ray前置），利用vless tcp回落/分流特性实现。

2、v2ray tcp类应用直连。v2ray ws类应用分流一次。naiveproxy回落(分流)一次。v2ray h2类应用回落一次，分流（反代）一次，共计两次。

3、caddy2 使用本人github文件，才可以同时支持naiveproxy及v2ray h2反向代理。
