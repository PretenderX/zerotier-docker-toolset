compose 文件中 [xxxxxxxxx] 自定义

所有镜像，dockerhub，github都可看原版文档

zerotier-ui必须第一位配置启动，然后建立网络
zerotier-moon和zerotier-router都是按照网络需求接入zerotier-ui建立的网络进行配置

要实现VPN的效果，需要将zerotier-router运行在对应的网络中，具体见内部readme

要加速国内访问，需要公网IP的服务器运行zerotier-moon，具体见内部readme

如果要完全与官方的控制器隔断（避免私有控制器频繁的反向代理请求），需要自建planet根节点文件然后替换zerotier-ui中dec0dos/zerotier-controller容器中的world.bin文件