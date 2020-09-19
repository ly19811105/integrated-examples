本配置采用v2ray自带shadowsocks协议及自身v2ray'分离'出的v2ray-plugin插件，直接实现了shadowsocks+v2ray-plugin应用，客户端直接使用shadowsocks即可。

另外通过caddy2实现ws反向代理，隐藏了数据。原理图： v2ray client <----- ws+tls ------> caddy2 <-- ws --> v2ray server
