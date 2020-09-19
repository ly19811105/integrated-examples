原理图：
v2ray client <--- tcp+tls ---> v2ray server <--- 回落 ---> caddy2

注意：

1、caddy2 目前只能json配置才能支持 h2c server，故要实现回落h2c就不能采用Caddyfile配置。

2、caddy2 支持http/1.1 h2c server共用一个端口。
