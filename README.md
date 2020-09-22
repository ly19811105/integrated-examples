这里是科学上网的集成配置示例。
如是不太了解科学上网，建议先依次从简单到复杂参考及部署。


单一集成服务器端配置示例（从简单到复杂）

1、v2ray(vless\vmess+ws+tls)+caddy2 （之前vmess协议时代，推荐部署。）

2、v2ray(vless\vmess+h2)+caddy2 （h2优势：链路复用。）

3、v2ray(SS+v2ray-plugin+tls)+caddy2（不常用，如需直接使用shadowsocks客户端可部署。）

4、v2ray(vless+tcp+tls)+caddy2 （vless协议新特性:tcp应用下的回落/分流）

5、v2ray(vless+tcp+tls+ws)+caddy2 （目前推荐部署，同时支持tcp与ws。）


综合集成服务器端配置示例（从简单到复杂）

1、v2ray(complete-tcp)+caddy2 （vless+ws、vless+h2、shadowsocks+ws、vmess+kcp+seed）

2、v2ray(complete)+caddy2 （vless+tcp、vless+ws、vless+h2、shadowsocks+ws、vmess+kcp+seed）

3、v2ray(complete)+naiveproxy （上一项应用+naiveproxy）

4、v2ray(complete)+naiveproxy+trojan（上一项应用+trojan。各程序监听端口对外公开，同级对等。）

  5、v2ray(complete)+naiveproxy+trojan+nginx （用nginx对上一项应用进行SNI分流，共用443端口。）

注：naiveproxy=caddy2+forwardproxy。此程序文件已编译好，本github下载即可。

贡献指南

欢迎你将自己使用的配置制作模板，提交 PR。
