通过caddy2或nginx前置v2ray server实现ws反向代理。

原理图： v2ray client <----- ws+tls ------> caddy2\nginx <- ws -> v2ray server
