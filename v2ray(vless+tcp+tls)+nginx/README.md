此配置实现以http/1.1或http/2自适应代理科学上网，非v2ray的web回落给nginx。

原理图： v2ray client <--- tcp+tls ---> v2ray server <--- web回落 ---> nginx

注意：

nginx 支持 h2c server，但不支持http/1.1 server与h2c server共用一个端口或一个进程。
