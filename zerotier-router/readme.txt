1.容器启动连入特定zerotier网络后，按照官方指引手动构建iptable规则：
https://docs.zerotier.com/route-between-phys-and-virt/
2.在zero-ui页面中对特定zerotier网络配置需要穿透的网络到zerotier-router容器zerotier 网络IP(以下简称：路由IP)的路由规则，比如192.168.1.*网段，配置 Target: 192.168.1.0/24    Via: 路由IP