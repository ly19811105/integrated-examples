原理图： v2ray client <----- H2 ------> caddy2 <-- H2C --> v2ray server

注意： caddy2 等于或大于v2.2.0-rc.1版才支持反向代理v2ray H2(HTTP/2) 应用，即caddy2支持
