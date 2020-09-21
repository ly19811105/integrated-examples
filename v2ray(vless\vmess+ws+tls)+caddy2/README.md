原理图： v2ray client <----- ws+tls ------> caddy2 <- ws -> v2ray server

通过caddy2前置v2ray server实现ws反向代理，隐藏了数据。
