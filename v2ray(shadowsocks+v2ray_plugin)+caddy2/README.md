本配置采用v2ray自带shadowsocks协议及自身v2ray分离出v2ray-plugin插件，实现了直接使用shadowsocks客户端应用。

另外通过caddy2实现ws反向代理，隐藏了数据。原理图： v2ray client <----- ws+tls ------> caddy2 <-- ws --> v2ray server
