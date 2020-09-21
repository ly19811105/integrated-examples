原理图： v2ray client <----- h2 ------> caddy2 <-- h2c --> v2ray server

注意： caddy2 等于或大于 v2.2.0-rc.1 版才支持反向代理v2ray H2(HTTP/2) 应用，即 caddy2 h2c proxy 应用。
