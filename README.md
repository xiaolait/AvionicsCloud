# 航点云demo
该demo包含端设备和云设备两部分，其中端设备由taget和weapon两个传统航电设备组成，目前由虚拟机实现；云设备由端设备代理服务和UI服务两个服务组成

1.端设备服务通过docker-compose.yaml文件管理两个端设备（需要将REDIS_SERVER改成本地ip地址）  
2.云设备服务通过deployment.yaml文件管理两个云服务（需要将RedisIp改成上面REDIS_SERVER地址）

两个设备可以部署在同一台PC，也可部署在两台PC。  
UI访问路径为：http://云设备ip地址:31080
