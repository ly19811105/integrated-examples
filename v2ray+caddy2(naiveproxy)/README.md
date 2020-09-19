注：

1、除v2ray kcp外,所用应用共用443端口。

2、v2ray tcp类应用直连。v2ray WS类应用分流一次。naiveproxy回落(分流)一次。v2ray h2类应用回落一次，分流（反代）一次，共计两次。
