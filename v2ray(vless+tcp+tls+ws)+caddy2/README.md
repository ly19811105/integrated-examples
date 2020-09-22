VLESS over TCP with TLS + 回落 & 分流 to WebSocket（tcp直连，web回落，ws分流。）

利用 VLESS TCP 强大的回落/分流特性，实现了 443 端口 VLESS over TCP with TLS 和任意 WS 的完美共存，而 WS 还可以 CDN 。

1_v2ray_config.json为VLESS TCP分流VLESS WS 配置，2_v2ray_config.json为VLESS TCP分流VMess WS 配置，3_v2ray_config.json为VLESS TCP分流shadowsocks WS 配置。
