这里是科学上网的集成配置示例。
如是不太了解科学上网，建议先依次从简单到复杂参考及部署。


单一集成配置示例（从简单到复杂）

1、v2ray(vless\vmess+ws+tls)+caddy2 （之前vmess协议时代，推荐部署。）

2、v2ray(vless\vmess+h2)+caddy2 （h2优势:链路复用。）

3、v2ray(SS+v2ray-plugin+tls)+caddy2（不常用，如需直接使用shadowsocks客户端可部署。）

4、v2ray(vless+tcp+tls)+caddy2 （vless协议新特性:tcp应用下的回落/分流）

5、v2ray(vless+tcp+tls+ws)+caddy2 （目前推荐部署，同时支持tcp与ws。）


综合集成配置示例（从简单到复杂）

1、v2ray(complete)+caddy2 （vless+tcp、vless+ws、shadowsocks+ws、vless+h2、vmess+kcp+seed）

2、v2ray(complete)+naiveproxy （上述应用+naiveproxy）

3、v2ray(complete)+naiveproxy+trojan（上述应用+trojan）

4、v2ray(complete)+naiveproxy+trojan+nginx （用nginx来对v2ray、naiveproxy、trojan分流，实现共用一个端口，如443端口。）


贡献指南

欢迎你将自己使用的配置制作模板，提交 PR。
