这里是科学上网的集成配置示例。
如是不太了解科学上网，建议先依次从简单到复杂参考及部署。


单一集成配置示例（从简单到复杂）

1、v2ray(vless\vmess+ws+tls)+caddy2 （老vmess协议时代，推荐部署。）

2、v2ray(vless\vmess+h2)+caddy2 （老vmess协议时代，推荐部署。）

3、v2ray(SS+v2ray-plugin+tls)+caddy2（不常用，如需直接使用shadowsocks客户端可部署。）

4、v2ray(vless+tcp+tls)+caddy2 （vless协议新特性（回落/分流））

5、v2ray(vless+tcp+tls+ws)+caddy2 （目前推荐部署，同时支持TCP与WS。）


综合集成配置示例

1、v2ray(complete)+caddy2

2、v2ray(complete)+naiveproxy

3、v2ray(complete)+naiveproxy+trojan

4、v2ray(complete)+naiveproxy+trojan+nginx


贡献指南
欢迎你将自己使用的配置制作模板，提交 PR。
