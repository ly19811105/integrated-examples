此配置实现以http/1.1或http/2自适应代理科学上网，非v2ray的web回落给caddy2。

原理图：
v2ray client <--- tcp+tls ---> v2ray server <--- web回落 ---> caddy2

注意：

1、caddy2 目前只能json配置才支持 h2c server，故要实现回落h2就不能采用Caddyfile配置。

2、caddy2 支持http/1.1 server与h2c server共用一个端口。
