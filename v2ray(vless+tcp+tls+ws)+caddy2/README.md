VLESS over TCP with TLS + 回落 & 分流 to WebSocket

利用 VLESS 强大的回落分流特性，实现了 443 端口 VLESS over TCP with TLS 和任意 WS 的完美共存及WS可以CDN。


原理图： v2ray client <--- tcp/ws+tls ---> v2ray server <--- 回落 ---> caddy2

                                              \<--- 分流 ---> v2ray server
注意：

1、caddy2 目前只能json配置才能支持 h2c server，故要实现回落h2c就不能采用Caddyfile配置。

2、caddy2 支持http/1.1 h2c server共用一个端口。


config_server_1.json为分流VLESS WS，config_server_2.json为分流VMess WS，config_server_3.json为分流shadowsocks WS。
