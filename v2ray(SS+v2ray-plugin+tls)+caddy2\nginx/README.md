本配置采用v2ray自带shadowsocks协议及自身v2ray'分离'出的v2ray-plugin插件，直接实现了shadowsocks+v2ray-plugin应用，客户端直接使用shadowsocks即可。

另外通过caddy2\nginx前置v2ray server实现ws反向代理，隐藏了数据。原理图： v2ray client <----- ws+tls ------> caddy2\nginx <- ws -> v2ray server
