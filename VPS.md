# Visual Personal Server搭建
##流程
Vultr注册和购买
Xshell 5下载和安装
ShadowSocksR安装和配置
客户端安装和配置
##详细内容
大部分内容可以直接参考[VPS教程](http://vultr.aicnm.com/Vultr-VPS%E4%B8%BB%E6%9C%BA%E5%BF%AB%E9%80%9F%E5%AE%89%E8%A3%85Shadowsocks%EF%BC%88ss%EF%BC%89%E5%AE%8C%E6%95%B4%E5%9B%BE%E6%96%87%E6%95%99%E7%A8%8B/ "VPS教程")
##Xshell 5破解
因为这软件下载之后就要你自动更新，否则不能使用，可以参考教程停止自动更新
[Xshell 5强制更新解决](https://www.banwagongzw.com/106.html "Xshell 5强制更新解决")
##ShadowSocksR配置
```shell
#按照VPS教程中配置好SSR之后，可以对配置文件进行修改以满足多用户的需求
vi /etc/shadowsocks.json
#修改后重启服务
/etc/init.d/shadowsocks restart
#可以通过stats检查端口开放状态
netstat -ntlp
```
```shell
#如果netstat没有安装，则需要先安装
yum install net-tools
```